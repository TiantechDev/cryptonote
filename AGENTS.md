# Agent instructions — cryptonote

## TianTech GitHub & AI Engineering Standard (organization policy)

- Default GitHub organization is `TiantechDev` (https://github.com/TiantechDev). Use `kaptangece53` only for explicitly personal or legacy references. Verify repository and branch before any write.
- Prefer the connected GitHub Agent for inspection, focused edits, commits and pull requests. Use GitHub CLI for unsupported administration only; avoid unnecessary user-side commands.
- Use Codex only when substantial software engineering, complex debugging or multi-file refactoring requires it. Read only task-relevant files and context, avoid repeat repository-wide scans, and keep responses concise.
- Use included, verified GitHub Enterprise features where helpful. Never activate paid add-ons, new licenses, metered usage or billing without explicit user approval.
- Keep GitHub Actions runner consumption minimal, preserve manual execution preferences, and do not trigger workflows for documentation-only work. Do not change workflow triggers without assessing impact.
- Never deploy production, publish releases, modify DNS, rotate live secrets or change production access without explicit authorization.
- Follow least privilege, protect secrets and confidential data, and respect branch protection, review requirements and environment policies.
- Make changes minimal, testable and reversible. Preserve repository-specific `AGENTS.md`, nested rules, architecture documents and established workflows; if conflicts arise, report them rather than silently overriding safeguards.
- First verify current state, avoid repeating confirmed research or already-successful tests, and run only relevant validation. Report completed changes, verification, checks not run, and remaining risks.

## Varsayılan Graphify çalışma standardı

- Her yazılım geliştirme görevinin başında proje kökünde `graphify-out/graph.json` dosyasını ve grafiğin güncelliğini kontrol et. Grafiğin kayıtlı kaynak revizyonunu mevcut `HEAD` ile ve analiz kapsamındaki çalışma ağacı değişiklikleriyle karşılaştır. Güncellik kanıtı yoksa grafiği güncel sayma.
- Mimari analiz, çağrı ilişkileri ve bağımlılık keşfinde güncel Graphify grafiğini önce sorgula. Yalnız görevle ilgili kaynak dosyalarını oku ve kritik çıkarımları bu dosyalardan doğrula.
- Grafik güncelse yeniden analiz etme. Kod değişikliklerinden sonra proje kökünden yerel grafiği güncelle, grafik çıktısını kontrol et ve analiz edilen kaynak durumunu kaydet.
- Yerel Graphify 0.9.120 ile `GRAPHIFY_BACKEND=none graphify extract . --code-only` kullan. Rapor ve HTML gerektiğinde `GRAPHIFY_BACKEND=none graphify cluster-only . --no-label` çalıştır. Projenin `.graphifyignore` kurallarını uygula. Secret, kimlik bilgisi, özel anahtar, `.env`, müşteri veya üretim verisi, log ve yedekleri kapsam dışında tut. Graphify Cloud veya harici LLM kullanma. Hassas çıktıları açık depolarda yayımlama.
- Grafik yoksa, eskiyse veya erişilemiyorsa ve güvenli yerel güncelleme mümkün değilse doğrudan gerekli kaynak kodu incele. Sonuçta grafik durumunu ve kısıtı belirt. Bu standart, kullanıcı Graphify’ı ayrıca anmasa da geçerlidir.

