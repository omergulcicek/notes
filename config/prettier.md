# Prettier Konfigürasyonu

## .prettierrc Dosyası İçeriği

```json
{
	"singleQuote": false,
	"semi": false,
	"useTabs": true,
	"tabWidth": 2,
	"printWidth": 80,
	"trailingComma": "none",
	"endOfLine": "auto",
	"arrowParens": "always",
	"quoteProps": "as-needed",
	"ObjectCurlySpacing": "always",
	"explicitTypes": "always",
	"HTMLWhitespaceSensitivity": "ignore",
	"importOrder": [
		"^(react/(.*)$)|^(react$)|^(react-(.*)$)",
		"^(next/(.*)$)|^(next$)|^(next-(.*)$)",
		"^(@next)/(.*)$",
		"",
		"^(@tanstack)/(.*)$",
		"<THIRD_PARTY_MODULES>",
		"",
		"^@/types",
		"",
		"^@/providers",
		"^@/layouts",
		"^@/components",
		"^@/ui",
		"^@/ag",
		"^@/widgets",
		"^@/shared",
		"^@/skeletons",
		"",
		"^@/stores",
		"^@/services",
		"",
		"^@/hooks",
		"^@/utils",
		"",
		"^@/data",
		"^@/img",
		"",
		"^[./]"
	],
	"importOrderSeparation": true,
	"importOrderSortSpecifiers": true,
	"importOrderCaseInsensitive": true,
	"plugins": [
		"@ianvs/prettier-plugin-sort-imports",
		"prettier-plugin-tailwindcss"
	]
}
```

## Ayar Açıklamaları

### Temel Formatlar
- `singleQuote: false` - Çift tırnak kullan
- `semi: false` - Noktalı virgül kullanma
- `useTabs: true` - Tab karakteri kullan
- `tabWidth: 2` - Tab genişliği 2 karakter
- `printWidth: 80` - Satır uzunluğu maksimum 80 karakter

### Import Sıralaması
1. React kütüphaneleri
2. Next.js kütüphaneleri
3. Third-party modüller
4. Tip tanımları (@/types)
5. Providers, layouts, components
6. Stores, services
7. Hooks, utils
8. Data ve assets
9. Relative imports

## Gerekli Paketler
```bash
npm install --save-dev @ianvs/prettier-plugin-sort-imports prettier-plugin-tailwindcss
``` 