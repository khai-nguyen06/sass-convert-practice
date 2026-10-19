# sass-convert-practice-a

Bài thực hành chuyển đổi CSS truyền thống sang SCSS theo cấu trúc chuẩn.

## Cấu trúc thư mục

```
sass-convert-practice-a/
├── css/
│   └── styles.css          # File CSS gốc
├── scss/
│   ├── abstracts/
│   │   ├── _variables.scss # Biến màu sắc, shadow
│   │   └── _mixins.scss    # button-style, box-shadow
│   ├── base/
│   │   └── _global.scss    # Style cho body
│   ├── layout/
│   │   └── _container.scss # .container
│   ├── components/
│   │   ├── _buttons.scss   # .button (có nesting &:hover)
│   │   └── _cards.scss     # .card
│   └── main.scss           # Import toàn bộ partials
├── dist/
│   └── main.css            # CSS biên dịch từ main.scss
└── package.json
```

## Biên dịch

```bash
npm install
npm run build   # scss/main.scss -> dist/main.css
npm run watch   # tự động biên dịch khi lưu file
```
