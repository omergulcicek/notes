# IDE Cache Sorunları Çözümleri

## Problem
Komut satırında hata yok ama IDE'de hatalar görünüyor.

## Terminal Komutları (Cache Temizleme)

### Cache Temizleme Komutları
```bash
rm -rf .eslintcache
rm -rf node_modules/.cache
rm -rf .next
```

### TypeScript Kontrol Komutu
```bash
npx tsc --noEmit
```

## IDE Çözüm Adımları

1. **Editörü tamamen kapat**

2. **Editörü tekrar aç**

3. **TypeScript Language Server'ı yeniden başlat**
   - `Cmd+Shift+P` (macOS) / `Ctrl+Shift+P` (Windows/Linux)
   - "TypeScript: Restart TS Server"

4. **ESLint Server'ı yeniden başlat**
   - `Cmd+Shift+P` (macOS) / `Ctrl+Shift+P` (Windows/Linux)
   - "ESLint: Restart ESLint Server"

5. **Editörü reload et** (son çare)
   - `Cmd+Shift+P` (macOS) / `Ctrl+Shift+P` (Windows/Linux)
   - "Developer: Reload Window"

## Not
Bu komutlar global terminal komutları değil, proje bazlı cache temizleme komutlarıdır. Her proje klasöründe çalıştırılmalıdır. 