# Microsoft Copilot 365

## 🛠 Faza 1: Fundamenty i Bezpieczeństwo Danych (Pre-Deployment)
Zanim zaimplementujesz AI, upewnij się, że Twoje dane są uporządkowane i bezpieczne.

| Obszar | Punkt Kontrolny | Narzędzie | Działanie Techniczne |
| --- | --- | --- | --- |
| Klasyfikacja | Sensitivity Labels | MS Purview | Włącz Auto-labeling, aby system sam oznaczał pliki zawierające np. numery kont lub dane osobowe, aby Copilot wiedział, co wymaga szczególnej ochrony. |
| Retencja | Data Minimization | Purview Compliance | Skonfiguruj Retention Policies. Usuń stare, nieaktualne procedury z SharePoint, aby uniknąć halucynacji AI. |
| Dostęp | Least Privilege | SharePoint Admin | Uruchom raport Data Access Governance. Zlikwiduj uprawnienia "Wszyscy" (Everyone) dla witryn wrażliwych i zamień je na grupy dedykowane. |
| Admin | Just-In-Time Access | Entra ID (PIM) | Włącz Privileged Identity Management. Dostęp administracyjny do Copilota tylko na czas wykonania zadania. |

## 🏗 Faza 2: Konfiguracja i Integracja (Implementation)
Zabezpieczenie "mózgu" AI (Copilot Studio) oraz punktów styku z aplikacją webową.

| Obszar | Punkt Kontrolny | Narzędzie | Działanie Techniczne |
| --- | --- | --- | --- |
| Knowledge | Grounding Scope | Copilot Studio | Ogranicz zakres Generative Answers wyłącznie do specyficznych folderów SharePoint/OneDrive (nie cały tenant). |
| Tożsamość | App Registration | Entra ID | Ustaw uprawnienia typu Delegated (Sites.Selected). Copilot może widzieć tylko to, co widzi dany użytkownik. |
| Web Security | Content Security Policy | Web Server / App Header | Skonfiguruj nagłówek CSP frame-ancestors, aby zapobiec atakom Clickjacking na okno czatu Copilota w Twojej aplikacji. |
| Auth Flow | On-Behalf-Of (OBO) | Entra ID / MSAL.js | Skonfiguruj przepływ OBO, aby aplikacja webowa bezpiecznie wymieniała token użytkownika na token dla Copilot Studio (brak konieczności drugiego logowania). |

## 🔍 Faza 3: Monitoring i Audyt (Post-Deployment)

| Obszar | Punkt Kontrolny | Narzędzie | Działanie Techniczne |
| --- | --- | --- | --- |
| Dostęp Warunkowy | Conditional Access | Entra ID | Wymuś politykę: Dostęp do Copilota = MFA + Zaufane Urządzenie (Intune Compliant). |
| Reakcja | CAE (Continuous) | Entra ID | Włącz Continuous Access Evaluation, aby natychmiast blokować sesję AI po wyłączeniu konta lub zmianie lokalizacji. |
| Audyt | Logowanie zapytań | Purview | Włącz Unified Audit Log. Upewnij się, że masz licencję (E3/E5), która pozwala na retencję logów Copilota powyżej 90 dni. Rejestruj każde zapytanie (Prompt) wysłane do Copilota w celach audytowych. |
| Monitoring | Prompt Injection | Sentinel | Podłącz konektor Microsoft 365 do Sentinela. Zaimportuj gotowe reguły analityczne (NRT - Near Real Time) dla Microsoft Copilot do wykrywania Prompt Injection lub masowego eksportu danych przez AI. |
| Monitoring | Ochrona przed Malware | Defender for O365 | Skonfiguruj alerty na złośliwe linki/pliki przesyłane w czatach (szczególnie przy użyciu zewnętrznych wtyczek/pluginów). |
| DLP | Clipboard & Export Protection | Purview Endpoint DLP | Zablokuj możliwość kopiowania wrażliwych odpowiedzi z Copilota do aplikacji niezarządzanych (np. prywatny Gmail, Notatnik) na komputerach pracowników. |