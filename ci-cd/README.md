# CI/CD

## CI/CD nima?

![DevOps](/imagesMarkdown/CICD-devops-1024x536.webp)

CI/CD (Continuous Integration / Continuous Delivery) — bu kodni kommitdan ishlab chiqarishga yetkazish jarayonini avtomatlashtiruvchi amaliyotlar va vositalar to‘plami.

Qisqacha aytganda:  
**kodni push qildingiz → pipeline ishladi → natija oldindan aytib bo‘ladigan**.  
Hech qanday “qo‘lda qilaylik”, “mening mashinamda ishlaydi” kabi “sehrli” jarayonlarsiz.

---

## Nima uchun kerak

CI/CD bir vaqtning o‘zida bir nechta tizimli muammolarni hal qiladi:

- qo‘lda ishlashni kamaytiradi  
- deploy xatolarini kamaytiradi  
- o‘zgarishlarni tezroq yetkazadi  
- jarayonni takrorlanadigan qiladi  

Asosiy qiymati — **barqarorlik va qayta takrorlash imkoniyati**, tezlik uchun tezlik emas.

---

## Tarkibi

Oddiy CI/CD pipeline quyidagi bosqichlardan iborat:

1. **Source**  
   - repositoryga push / merge / tag

2. **Build**  
   - ilovani yig‘ish  
   - artefaktlar yoki Docker-imagellar yaratish

3. **Test**  
   - unit / integration testlar  
   - statik analiz

4. **Deploy**  
   - staging yoki productionga deploy  
   - avtomatik yoki manual approval bilan

---

## Qayerda ishlatiladi

- shaxsiy loyihalar (pet-project)  
- startaplar  
- korporativ tizimlar (enterprise)  
- Kubernetes yoki klassik VMlar  

CI/CD bitta servis uchun ham, yuzlab mikroservislar uchun ham zarur.

---

## Mashhur vositalar

- GitHub Actions — oddiy va tez, alohida infra kerak emas  
- GitLab CI/CD — kuchli, hamma narsa bitta joyda  
- Jenkins — moslashuvchan, lekin intizom talab qiladi  
- Argo CD — GitOps va Kubernetes uchun

Qaysi vositani tanlash ikkinchi darajali.  
**Muhimi pipeline mavjud va ishonchli bo‘lishi.**

---

## CI/CD bo‘lmasa nima bo‘ladi

- deploy Confluence’dagi ko‘rsatmalarga qarab  
- “oxirgi kim deploy qildi?” savoli  
- tuzatishlarni to‘g‘ridan-to‘g‘ri productionga kiritish  
- reliz = stress va panika

---

## Xulosa

CI/CD — bu YAML haqida emas.  
Bu — nazorat, qayta takrorlash va oldindan aytib bo‘ladigan jarayonlar haqida.

Agar deploy hodisa bo‘lsa, demak CI/CD noto‘g‘ri sozlangan.

---

## Mem (majburiy qism)

> **Deploy juma kuni.**  
> *Nima xato bo‘lishi mumkin?* 
![gif](https://www.reactiongifs.us/wp-content/uploads/2013/10/nuh_uh_conan_obrien.gif)

⬇️  
![DevOps](/imagesMarkdown/serverisdown.jpg)
