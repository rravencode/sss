# Tarih yerelleştirme nasıl yapılır?

TypeScript için:

```ts
const date: Date = new Date();
// "tr-TR" yazan yer dil seçeneği
const trDate: string = date.toLocaleDateString("tr-TR", {
  weekday: "long",
  month: "long",
  year: "numeric",
  day: "numeric",
});

console.log(trDate); //-> 27 Mart 2023 Pazartesi
```

JavaScript için:

```js
const date = new Date();
// "tr-TR" yazan yer dil seçeneği
const trDate = date.toLocaleDateString("tr-TR", {
  weekday: "long",
  month: "long",
  year: "numeric",
  day: "numeric",
});

console.log(trDate); //-> 27 Mart 2023 Pazartesi
```
