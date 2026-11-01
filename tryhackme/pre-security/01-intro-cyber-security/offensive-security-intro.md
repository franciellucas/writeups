## Offensive Security Intro · 01/11/2026 · <tempo gasto:20 minutos>
- Em 1 frase: esconder uma página não é proteger; sem autenticação, qualquer um que a encontre pode usá-la (controle de acesso quebrado, OWASP A01).
- Comandos/ferramentas: `dirb <url>`: testa nomes de uma wordlist e lista com "+" o que não retorna 404.
- No Blue Team isso aparece em: log de acesso web com rajada de 404 do mesmo IP em segundos, seguida de 200 numa página sensível. ATT&CK T1595.003 (Wordlist Scanning).
- Liga com meu plano: T6 (regra: pico de 404 por IP); T2 PortSwigger (access control); mitigação: autenticação + rate limiting/WAF.
- Revisar: como fica uma linha de log de acesso do Apache/Nginx (ver no homelab).
