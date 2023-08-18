# Fullstack Coding Test

Instructions:
- Clone this repository.
- Go to https://webhook.site/
- Set-up our env
- running the server; npm run dev
- Test the endpoint with this command; npx ts-node src/get-process.test.ts
- Explain what the program does, if you find a bug, provide the solution.
- You can explain by add more line in this file. if you needed to modify the program, feel free.
- push this repo to your private repository and add our github account as colaborator when you finish your work.

![alt text](1.png)


1. Program menerima data request yang akan dikirim ke webhook.site. Data berupa ID, email, nama, phone number. Sebelum data dikirim ke webhook.site, data request di validasi. Data yang divalidasi ada 2, yaitu ID dan data. Didalam data ada object yaitu email, nama dan phone number.
2. ID yang diterima dari request dengan ID yang dikirimkan ke webhook.site berbeda. Karena data ID yang diterima dari reqeust tidak dipakai, melainkan program melakukan random UUID.
3. Dilakukan penambahan validasi untuk properti ID, dan properti ID yang diterima dari request akan dikirimkan ke webhook.site. Sehingga ID yang diterima dari request akan sama dengan yang diterima webhook.site. Validasi berupa penambahan bahwa properti ID IsString, IsNotEmpty dan required (id!)