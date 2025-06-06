# 🛡️ Blacklists para Pi-hole e DNS/Web Filters

Bem-vindo ao repositório de **listas negras (blacklists)** mantidas pela comunidade para uso com o [Pi-hole](https://pi-hole.net/), [AdGuard Home](https://adguard.com/en/adguard-home/overview.html), e outros sistemas de filtragem de DNS/web.

Este projeto visa facilitar o bloqueio de anúncios, rastreadores, sites maliciosos, conteúdo adulto e outras categorias indesejadas por meio de listas atualizadas e organizadas.

---

## 🛡️ Pi-Hole - Listas Disponíveis

| Categoria             | Descrição                                                 | Link Direto                                                                                 |
|-----------------------|-----------------------------------------------------------|-------------------------------------------------------------------------------------------|
| **Anúncios**          | Bloqueia domínios usados por redes de publicidade         | [Anuncios](https://raw.githubusercontent.com/Thiago-Boaventura/IBR-Hospital/refs/heads/main/Backlists/Pi-Hole/anuncios)          |
| **Rastreadores**      | Impede o rastreamento de usuários                         | [Rastreadores](https://raw.githubusercontent.com/Thiago-Boaventura/IBR-Hospital/refs/heads/main/Backlists/Pi-Hole/rastreadores)      |
| **Malware/Phishing**  | Bloqueia domínios maliciosos e de phishing                | [Malware/Phishing](https://raw.githubusercontent.com/Thiago-Boaventura/IBR-Hospital/refs/heads/main/Backlists/Pi-Hole/malware)           |
| **Conteúdo adulto**   | Restringe acesso a conteúdo impróprio                     | [Adulto](https://raw.githubusercontent.com/Thiago-Boaventura/IBR-Hospital/refs/heads/main/Backlists/Pi-Hole/adulto)            |
| **Redes sociais**     | Bloqueia redes sociais específicas                        | [Redes Sociais](https://raw.githubusercontent.com/Thiago-Boaventura/IBR-Hospital/refs/heads/main/Backlists/Pi-Hole/redes_sociais)     |
| **Whatsapp**          | Bloqueia/Libera Whatsapp                                  | [Whatsapp](https://raw.githubusercontent.com/Thiago-Boaventura/IBR-Hospital/refs/heads/main/Backlists/Pi-Hole/whatsapp)          |
| **Jornais**           | Bloqueia/Libera Jornais/Portais/Blogs                     | [Portais](https://raw.githubusercontent.com/Thiago-Boaventura/IBR-Hospital/refs/heads/main/Backlists/Pi-Hole/portais)          |

## 🛡️ AdGuard Home - Listas Disponíveis 

| Categoria             | Descrição                                                 | Link Direto                                                                                 |
|-----------------------|-----------------------------------------------------------|-------------------------------------------------------------------------------------------|
| **Anúncios**          | Bloqueia domínios usados por redes de publicidade         | [Anuncios](https://raw.githubusercontent.com/Thiago-Boaventura/IBR-Hospital/refs/heads/main/Backlists/ADGuard/anuncios)          |
| **Rastreadores**      | Impede o rastreamento de usuários                         | [Rastreadores](https://raw.githubusercontent.com/Thiago-Boaventura/IBR-Hospital/refs/heads/main/Backlists/ADGuard/rastreadores)      |
| **Conteúdo adulto**   | Restringe acesso a conteúdo impróprio                     | [Adulto](https://raw.githubusercontent.com/Thiago-Boaventura/IBR-Hospital/refs/heads/main/Backlists/ADGuard/adulto)            |
| **Redes sociais**     | Bloqueia redes sociais específicas                        | [Redes Sociais](https://raw.githubusercontent.com/Thiago-Boaventura/IBR-Hospital/refs/heads/main/Backlists/ADGuard/redes_sociais)     |
| **Jornais**           | Bloqueia/Libera Jornais/Portais/Blogs                     | [Portais](https://raw.githubusercontent.com/Thiago-Boaventura/IBR-Hospital/refs/heads/main/Backlists/ADGuard/portais)          |


> ⚠️ **Use apenas as listas que forem adequadas ao seu ambiente.** Algumas podem impactar o funcionamento de serviços legítimos. Estas listas podem ser utilizadas tantao para bloquear quando liberar.

---

## 🚀 Como usar com o Pi-hole

1. Acesse a interface de administração do seu Pi-hole.
2. Vá até **Group Management > Adlists**.
3. Clique em **Add a new adlist**.
4. Cole o link da lista desejada.
5. Clique em **Add**.
6. Atualize as listas com o comando:

```bash
pihole -g
```

## 🚀 Como usar com o AdGuard Home

1. Acesse a interface de administração do seu AdGuard Home.
2. Vá até **Filtros > Listas de Bloqueio DNS**.
3. Clique em **Adicionar lista de bloqueio**.
4. Clique em **Adicionar uma lista personalizada**.
5. Cole o link da lista desejada.
6. Clique em **Add**.

```bash

```


---

## 💡 Dicas de uso

- Adicione apenas listas que sejam relevantes para o seu caso de uso.
- Verifique se a lista não está bloqueando domínios essenciais (ex: serviços de e-mail ou bancos).
- Combine listas com **whitelists personalizadas** para restaurar domínios legítimos.
- Teste o impacto em redes de produção com cautela.
- Ferramentas como o [FTL Logs](https://docs.pi-hole.net/ftldns/logs/) podem ajudar a identificar bloqueios indevidos.

---

## 🤝 Contribuindo

Contribuições são bem-vindas! Você pode:

- Criar uma **Issue** com domínios que devem ser incluídos ou removidos.
- Enviar um **Pull Request** com sugestões de novas listas ou atualizações.
- Usar fontes confiáveis e realizar verificações com ferramentas como [VirusTotal](https://www.virustotal.com/) e [URLHaus](https://urlhaus.abuse.ch/).

---

## 📅 Atualizações

As listas são mantidas com frequência e recebem:

- Revisões periódicas para evitar falsos positivos.
- Adição de novas fontes conforme surgem novas ameaças.
- Organização por categorias específicas para maior controle.

Fique de olho na aba **Commits** para acompanhar o histórico.

---

## 📄 Licença

Este projeto está licenciado sob a [MIT License](LICENSE).  
Você pode usar, modificar e distribuir com liberdade, desde que mantenha os créditos e os termos da licença.

---

## 🌐 Links úteis

- [Pi-hole Documentation](https://docs.pi-hole.net/)
- [AdGuard Home](https://github.com/AdguardTeam/AdGuardHome/wiki)
- [dnscrypt-proxy blocklists](https://github.com/DNSCrypt/dnscrypt-proxy/wiki/Block-lists)
- [StevenBlack Hosts](https://github.com/StevenBlack/hosts) – Uma das maiores fontes de listas unificadas.
- [Firebog Recommended Lists](https://firebog.net/) – Curadoria de listas confiáveis para Pi-hole.

---

👤 Thiago Boaventura  
🏥 IBR Hospital  
📍 Vitória da Conquista - Bahia  

