# DevSecOps / AppSec Mülakat Soru Seti

## 🔴 Client-Side Attacks

| # | Soru | Seviye |
|---|------|--------|
| 1 | XSS nedir? Stored vs Reflected vs DOM-based farkı ne? | Junior |
| 2 | XSS'den nasıl korunursunuz? CSP olmadan önlem alabilir misiniz? | Junior |
| 3 | Clickjacking nedir, nasıl exploit edilir? X-Frame-Options yeterli mi? | Junior |
| 4 | SOP (Same Origin Policy) CSRF'yi önler mi? Neden önlemez/önler? | Mid |
| 5 | CSRF saldırısından nasıl korunursunuz? SameSite cookie ne işe yarar? | Mid |
| 6 | Third-party JS kütüphanesinden malware gelirse nasıl savunursunuz? SRI nedir? | Mid |
| 7 | Open redirect nedir, nasıl korunursunuz? | Junior |

## 🟤 Injection Attacks

| # | Soru | Seviye |
|---|------|--------|
| 8 | SQL Injection nasıl çalışır? Prepared statement her zaman yeterli mi? | Junior |
| 9 | SQL Injection'dan nasıl korunursunuz? ORM kullanmak güvenli midir? | Junior |
| 10 | Command injection nedir, nasıl exploit edilir? | Mid |
| 11 | Command injection'dan nasıl korunursunuz? | Mid |
| 12 | SSTI (Server-Side Template Injection) nedir? Hangi senaryolarda ortaya çıkar? | Mid |
| 13 | XXE nedir? External entity neden tehlikelidir? Nasıl önlenir? | Mid |
| 14 | SSRF nedir? Cloud ortamında metadata endpoint'i nasıl abuse edilir? | Mid |
| 15 | SSRF'den nasıl korunursunuz? Allowlist yeterli midir? | Mid |

## 🟠 Authentication & Authorization

| # | Soru | Seviye |
|---|------|--------|
| 16 | AuthN ve AuthZ farkı nedir? Gerçek hayatta nasıl ayrılır? | Junior |
| 17 | JWT token nedir? Hangi saldırılar mümkündür? (alg:none, weak secret) | Mid |
| 18 | JWT'yi nasıl güvenli kullanırsınız? Token revocation nasıl yapılır? | Mid |
| 19 | OAuth2 authorization code flow'unu anlatın. PKCE ne için kullanılır? | Mid |
| 20 | OAuth2 misconfiguration'dan nasıl korunursunuz? | Mid |
| 21 | Broken Access Control nedir? IDOR örneği verir misiniz? | Junior |
| 22 | Broken Access Control'den nasıl korunursunuz? | Mid |
| 23 | Brute force ve credential stuffing farkı nedir? Nasıl korunursunuz? | Junior |
| 24 | Session hijacking nasıl gerçekleşir? Cookie flag'leri nasıl ayarlanmalı? | Mid |
| 25 | Password hash migration nasıl yapılır? (Node.js örneği üzerinden) | Mid |

## 🟡 Secure Development / SSDLC

| # | Soru | Seviye |
|---|------|--------|
| 26 | Threat modeling nedir? ATM makinesi için nasıl yaparsınız? (STRIDE) | Mid |
| 27 | Bir REST API için threat model nasıl oluşturursunuz? | Senior |
| 28 | SAST kaynak kodu görüyor, DAST'a ne gerek var? | Mid |
| 29 | DAST ile SSRF nasıl detect edilir? | Mid |
| 30 | CI/CD pipeline'ına hangi security check'leri eklersiniz? | Mid |
| 31 | Git history'de secret sızdıysa ne yaparsınız? | Mid |
| 32 | SCA toolundan gelen CVE'leri nasıl triaj edersiniz? Severity mi exploitability mi? | Senior |

## 🟢 Supply Chain & Dependency Security

| # | Soru | Seviye |
|---|------|--------|
| 33 | Dependency confusion saldırısı nedir? Nasıl gerçekleşir? | Mid |
| 34 | Dependency confusion'dan nasıl korunursunuz? | Mid |
| 35 | Malicious npm/pip package'dan nasıl korunursunuz? | Mid |
| 36 | SBOM nedir? Ne zaman ve neden üretilmeli? | Senior |
| 37 | Yeni bir third-party library eklemeden önce ne kontrol edersiniz? | Mid |
| 38 | Gerçek bir supply chain saldırısını anlatın. (XZ Utils, event-stream, vb.) | Senior |

## ☁️ Cloud Native / Kubernetes / Infrastructure

| # | Soru | Seviye |
|---|------|--------|
| 39 | Bash script'te secret'ları nasıl saklarsınız? Ne yapmamalısınız? | Junior |
| 40 | Secrets'ı CI/CD'de nasıl korursunuz? Vault/Conjur nasıl entegre edilir? | Mid |
| 41 | ConfigMap vs Secret farkı nedir? K8s'te secret oluşturmanın yolları nelerdir? | Junior |
| 42 | K8s'te sidecar pattern secret yönetimi için nasıl kullanılır? | Mid |
| 43 | K8s RBAC nasıl çalışır? Yaygın misconfiguration örnekleri nelerdir? | Mid |
| 44 | K8s cluster'ı nasıl sertleştirirsiniz? Pod Security Admission ne işe yarar? | Senior |
| 45 | Container escape nasıl gerçekleşir? Nasıl korunursunuz? | Senior |
| 46 | Container image'daki CVE'lerden nasıl korunursunuz? (Trivy, Grype) | Mid |
| 47 | Image signing nedir? Cosign/Notary neden kullanılır? | Senior |
| 48 | IRSA nedir? Static credential kullanmaktan neden daha güvenlidir? | Senior |
| 49 | Cloud storage (S3) yanlış konfigürasyonundan nasıl korunursunuz? | Mid |
| 50 | CI/CD pipeline'ını nasıl güvenli hale getirirsiniz? Pinned actions neden önemli? | Mid |

## 🤖 AI / Modern Threats

| # | Soru | Seviye |
|---|------|--------|
| 51 | Prompt injection nedir? Direct vs indirect farkı ne? | Mid |
| 52 | Prompt injection'dan nasıl korunursunuz? | Mid |
| 53 | LLM tabanlı uygulamada veri sızıntısı nasıl olur? Nasıl önlenir? | Senior |
| 54 | OWASP Top 10 for LLMs'i biliyor musunuz? En kritik 3'ünü açıklayın | Senior |

---

## 💡 Kullandığım Kategorizasyon

Her konuyu şu 3 katmanlı formatta sorabilirsiniz:

```
Katman 1 → "X nedir?"
           Kavramsal bilgiyi ölçer

Katman 2 → "X nasıl exploit edilir?"
           Saldırgan perspektifini ölçer
           (Savunma bilmek için saldırıyı anlamak gerekir)

Katman 3 → "X'den nasıl korunursunuz?"
           Pratik, uygulanabilir savunma bilgisini ölçer
```

**Örnek uygulama — XSS:**

1. "XSS nedir, kaç türü vardır?"
2. "DOM-based XSS'i nasıl exploit edersiniz?"
3. "CSP olmadan XSS'den nasıl korunursunuz?"

---

## 📊 Seviyeye Göre Soru Dağılımı

| Seviye | Soru Sayısı | Önerilen Konular |
|--------|-------------|------------------|
| Junior | 1-2-3, 8-9, 16, 21, 23, 39, 41 | Temel OWASP, Auth temelleri, K8s basics |
| Mid | 4-7, 10-15, 17-20, 22, 24-31, 33-36, 40, 42-43, 46, 49-52 | Threat model, CI/CD security, Cloud |
| Senior | 27, 32, 37-38, 44-45, 47-48, 53-54 | Architecture, Supply chain, AI, K8s hardening |
