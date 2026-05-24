# スクラム祭り ウェブサイト

このリポジトリは、スクラム祭りのウェブサイトのソースコードです。
Astro と Tailwind CSS を使用して構築されています。
（ベースとして [Astroship](https://github.com/surjithctly/astroship) テンプレートを利用しています）

> **⚠️ 注意事項**
> このサイトはサンプルページとして作成されています。
> 実際に運用（本番公開）する場合は、以下の作業を行ってください。
> - 実際の運用ドメインへの載せ替え（`astro.config.mjs` 等の設定や、ホスティング環境での独自ドメイン設定）
> - デプロイ環境（Vercel, Netlify, Cloudflare Pages, GitHub Pages 等）の構築・設定
> - お問い合わせフォームなど、必要に応じた動的機能のつなぎ込みや不要なサンプルページの削除
> - 本番向けのアクセス解析タグ（Google Analytics等）の設定
> - **ライセンスに関する注意**: 本リポジトリのソースコードはオープンソースとして公開されていますが、リポジトリ内に含まれる「企業ロゴ」や「スポンサーロゴ」等の画像アセットは各企業に著作権および商標権が帰属します。これらの画像アセットに関する無断転用や二次利用は固くお断りいたします。

## コンテンツの更新方法

### 1. 参加コミュニティの変更
参加コミュニティのデータは JSON ファイルで管理されています。
追加・変更・削除を行う場合は、以下のファイルを編集してください。
- **対象ファイル:** `src/content/communities.json`

### 2. Keynote スピーカーの変更
Keynote スピーカーの情報は、Astro コンポーネント内のデータ（配列）として管理されています。
スピーカーの追加・変更を行う場合は、以下のファイルの先頭にある `keynotes` 配列を編集してください。
- **対象ファイル:** `src/components/keynote.astro`

### 3. スポンサーの変更
スポンサーのロゴ情報は、プラン（Platinum, Gold, Silver, Bronze, 個人）ごとにコンポーネント内で管理されています。
スポンサーの追加・変更を行う場合は、以下のファイルの先頭にある `sponsors` 配列を編集してください。
- **対象ファイル:** `src/components/sponsors.astro`

### 4. サイト基本情報（SEO・OGP）の変更
サイトのタイトル、説明文、SNS共有時の画像（OGP）などを実際のイベントに合わせて変更してください。
- **対象ファイルの例:** `src/layouts/Layout.astro` や `src/components/seo.astro` などのレイアウト・SEO用コンポーネント

### 5. デザイン・配色のカスタマイズ
サイトのテーマカラーや基本デザインを変更する場合は、Tailwind CSS の設定を編集します。
- **対象ファイル:** `tailwind.config.cjs` （または `.mjs`）
- **ベーススタイル:** 基本となるCSSファイル（例: `src/styles/global.css` など）

---

## 開発サーバーの起動方法

```bash
# パッケージのインストール
npm install

# 開発サーバーの起動
npm run dev
```

---

*以下はベースとなった Astroship テンプレートのオリジナル README です。*

## Astroship - Astro SAAS Starter Website Template

<!-- prettier-ignore -->
| Feature | Free Version | Pro Version |
| --- | ------ | --- |
| Astro v3 | ✅  | ✅ |
| Content Collections | ✅  | ✅ |
| Tailwind CSS   | ✅  | ✅ |
| Mobile Responsive | ✅  | ✅ |
| Working Contact Page | ✅  | ✅ |
| Pro Layouts & Features | ❌  | ✅ |
| Blog with Pagination | ❌ | ✅ |
| View Transitions | ❌ | ✅ |
| Advanced Homepage Design | ❌  | ✅ |
| Features Page | ❌  | ✅ |
| Integrations Page | ❌  | ✅ |
| Elegant 404 Page | ❌  | ✅ |
| 6 Months Support| ❌  | ✅  |
| Free Updates    | ✅  | ✅  |
| License         | GPL-2.0 | Commercial |
| &nbsp; | &nbsp;| &nbsp;|
| Pricing| Free|**$49**|
| &nbsp; | [Deploy for free](https://vercel.com/new/surjithctly/clone?demo-description=Starter%20template%20for%20startups%2C%20marketing%20websites%20%26%20blogs%20built%20with%20Astro%20and%20TailwindCSS.&demo-image=%2F%2Fimages.ctfassets.net%2Fe5382hct74si%2F5dB0dDqBr1BfvIoNOmffVB%2F784984a8d3fe5e3db123e7c655166046%2Fastroship_-_Tony_Sullivan.jpg&demo-title=Astroship&demo-url=https%3A%2F%2Fastroship.web3templates.com%2F&from=templates&project-name=Astroship&repository-name=astroship&repository-url=https%3A%2F%2Fgithub.com%2Fsurjithctly%2Fastroship&skippable-integrations=1) | [Purchase Pro](https://web3templates.com/templates/astroship-pro-astro-saas-website-template) |

<a href="https://web3templates.com/templates/astroship-pro-astro-saas-website-template">
<img width="160" alt="Upgrade to Pro" src="https://user-images.githubusercontent.com/1884712/199181300-37c2128e-d033-4145-a906-16fa5263a53b.png">
</a>

## Deploy this template

You can instantly clone this to your GitHub and deploy the site by clicking the below buttons to deploy to your chosen providers!

Click here to deploy on Vercel:

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2Fsurjithctly%2Fastroship&project-name=astroship&repository-name=astroship&demo-title=Astroship%20-%20Astro%20Starter%20Template&demo-description=Astroship%20is%20a%20starter%20template%20for%20startups%2C%20marketing%20websites%20%26%20landing%20pages.%20Built%20with%20Astro%2C%20TailwindCSS&demo-url=https%3A%2F%2Fastroship.web3templates.com%2F&demo-image=https%3A%2F%2Fuser-images.githubusercontent.com%2F1884712%2F200831799-10ef2456-a02e-4068-b580-4b5326f0b33b.png)

Click here to deploy on Netlify:

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/surjithctly/astroship)

## Preview

![image](https://user-images.githubusercontent.com/1884712/200831799-10ef2456-a02e-4068-b580-4b5326f0b33b.png)

## Pro Version Preview

![preview](https://github.com/surjithctly/astroship/assets/1884712/25665c02-d2a7-43dc-89b2-34a8ae37ade9)

### Pagespeed Score

[![pagespeed](https://user-images.githubusercontent.com/1884712/210250214-7aa98167-7993-4b90-8138-326b8fa0c223.png)](https://pagespeed.web.dev/report?url=https%3A%2F%2Fastroship.web3templates.com%2F)

## Installation

If you are reading this on github, you can click on the "Use this template" button above to create a new repository from astroship to your account. Then you can do a `git clone` to clone it to your local system.

Alternatively, you can clone the project directly from this repo to your local system.

### 1. Clone the repo

```bash
git clone https://github.com/surjithctly/astroship.git myProjectName
# or
git clone https://github.com/surjithctly/astroship.git .
```

The `.` will clone it to the current directory so make sure you are inside your project folder first.

### 2. Install Dependencies

```bash
npm install
# or
yarn install
# or (recommended)
pnpm install
```

### 3. Start development Server

```bash
npm run dev
# or
yarn dev
# or (recommended)
pnpm dev
```

### Preview & Build

```bash
npm run preview
npm run build
# or
yarn preview
yarn build
# or (recommended)
pnpm preview
pnpm build
```

We recommend using [pnpm](https://pnpm.io/) to save disk space on your computer.

### Other Commands

```bash
pnpm astro ...
pnpm astro add
pnpm astro --help
```

## Project Structure

Inside of your Astro project, you'll see the following folders and files:

```
/
├── public/
│   └── ...
├── src/
│   ├── components/
│   │   └── ...
│   ├── layouts/
│   │   └── ...
│   └── pages/
│       └── ...
└── package.json
```

Astro looks for `.astro` or `.md` files in the `src/pages/` directory. Each page is exposed as a route based on its file name.

Any static assets, like images, can be placed in the `public/` directory.

## TailwindCSS

TailwindCSS is already configured in this repo, so you can start using it without any installation.

## Credits

[Hero Illustration](https://www.figma.com/community/file/1108400791662599811) by [Streamline](https://www.streamlinehq.com/)

## 👀 Want to learn more?

Feel free to check out [Astro Docs](https://docs.astro.build) or jump into our [Discord Chat](https://web3templates.com/discord).

[![Built with Astro](https://astro.badg.es/v1/built-with-astro.svg)](https://astro.build)
