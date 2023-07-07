This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.js`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/basic-features/font-optimization) to automatically optimize and load Inter, a custom Google Font.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.

## 需求

### GW2 貨幣計算機功能
- 批次新增很多筆 並把多筆加起來 自動進位
- gold 可以一位數以上 但silver,copper最多只能兩位數
- 乘法: 例如 23g 39s 88c 乘7等於多少? 可快速算出來
- 23g 39s 88c 這樣等於多少c? 可快速算出來
- 23g 39s 88c 這樣等於多少s? 可快速算出來
- 23g 39s 88c 這樣等於多少g? 可快速算出來
- 0g 39s 88c 這樣等於多少g? 要算出小數點
- 除法: 我有23g 39s 88c, 那waypoint一次要3s 74c, 那我可以傳幾次? 23g 39s 88c/3s 74c

### 算法

1g=100s
1s=100c
1g=10000c

1s=0.01g
1c=0.01s
1c=0.0001g
