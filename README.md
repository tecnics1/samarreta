# Votació de samarretes (GitHub Pages + Firebase)

## 1. Crea el projecte a Firebase (gratuït)
1. Ves a https://console.firebase.google.com → **Afegeix un projecte** (pots desactivar Analytics).
2. **Build → Authentication → Get started**. A *Sign-in method* activa **Anonymous** i **Email/Password**.
3. A *Users* → **Add user**: crea el teu correu i contrasenya d'administrador.
4. **Build → Firestore Database → Create database** (mode producció, qualsevol regió d'Europa).
5. A la pestanya **Rules**, enganxa el contingut de `firestore.rules` (canvia el correu pel teu) i **Publish**.
6. **Configuració del projecte (roda dentada) → Your apps → </> Web** → registra l'app i copia l'objecte `firebaseConfig`.
7. Enganxa'l a `index.html` (bloc marcat amb «ENGANXA AQUÍ»).
8. A **Authentication → Settings → Authorized domains** afegeix `EL-TEU-USUARI.github.io`.

## 2. Penja-ho a GitHub
1. Crea un repositori nou i puja `index.html` (el `firestore.rules` i aquest README són opcionals).
2. **Settings → Pages → Deploy from a branch → main / (root)**.
3. La votació estarà a `https://EL-TEU-USUARI.github.io/NOM-REPO/`.

## 3. Ús
- **Votants:** obren l'enllaç i voten. Sense comptes.
- **Admin:** obre `https://EL-TEU-USUARI.github.io/NOM-REPO/#admin`, entra amb el teu correu i afegeix/elimina candidats.
