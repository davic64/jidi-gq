# JIDI GQ (Representantes)

![Status](https://img.shields.io/badge/status-en%20desarrollo-FF6C76)
![Firebase](https://img.shields.io/badge/Firebase-backend-yellow)
![React](https://img.shields.io/badge/React-frontend-61DAFB)
![Zustand](https://img.shields.io/badge/Zustand-state%20management-blue)
![shadcn/ui](https://img.shields.io/badge/UI-shadcn%2Fui-FF6C76)

> PWA para representantes de jóvenes e iglesias. Gestión de asistencia, materiales, avisos y comunicación con estilo juvenil y funcionalidad optimizada para móvil y escritorio.

---

## ✨ Características principales

### 👤 Representantes de jóvenes

- 📋 Lista personalizada de jóvenes
- ✅ Registro de asistencia semanal
- 📈 Estadísticas visuales
- 📢 Avisos oficiales del administrador
- 📂 Descarga de materiales desde Google Drive
- 📞 Enlace directo a juntas por Jitsi Meet

### 🛠️ Administradores

- 👥 Gestión de representantes e iglesias
- 📣 Creación y envío de avisos
- 📊 Estadísticas globales de participación
- 📤 Subida de materiales y asignación a iglesias
- ⚙️ Configuración de enlaces de reunión

---

## 🛠️ Stack Tecnológico

| Tecnología          | Uso                               |
| ------------------- | --------------------------------- |
| **React + Vite**    | Frontend moderno                  |
| **TypeScript**      | Tipado estático                   |
| **Firebase**        | Auth, Firestore, Storage          |
| **Zod**             | Validaciones tipadas              |
| **React Hook Form** | Formularios y validaciones        |
| **Zustand**         | Manejo de estado global           |
| **shadcn/ui**       | Componentes accesibles + Tailwind |

---

## 🎨 Paleta de Colores

| Uso             | Color         | Hex       |
| --------------- | ------------- | --------- |
| Color principal | Coral         | `#FF6C76` |
| Fondo suave     | Rosa pastel   | `#FFE8E8` |
| Sidebar oscuro  | Azul grisáceo | `#1F1F2E` |
| Secundarios     | Lavanda       | `#D1B3FF` |
| Confirmaciones  | Verde         | `#2ECC71` |
| Alertas         | Rojo          | `#FF5C5C` |

---

## 📂 Estructura del Proyecto

```
src/
├── components/
│   ├── ui/             # Componentes base (shadcn)
│   ├── custom/         # Componentes propios (Navbar, Sidebar, etc.)
│   ├── layouts/        # Layouts reutilizables
│   ├── pages/          # Formularios, vistas
│
├── lib/
│   ├── hooks/          # useAuth, useUser, etc.
│   ├── helpers/        # Funciones utilitarias
│   ├── constants/      # Constantes globales
│   ├── types/          # Tipos TypeScript
│   ├── validators/     # Schemas de Zod
│   ├── store/          # Zustand store
│
├── services/           # Firebase logic
│   ├── firebase.ts
│   ├── auth.ts
│   ├── user.ts
│   ├── firestore.ts
│
├── pages/              # Páginas por rol
├── routes/             # Rutas protegidas y config
├── styles/             # Tailwind config y estilos
├── index.tsx
```

---

## 🚀 Cómo ejecutar localmente

1. Clona el repositorio:

   ```bash
   git clone https://github.com/davic64/jidi-gq.git
   cd jidi-gq
   ```

2. Instala las dependencias:

   ```bash
   yarn install
   ```

3. Configura las variables de entorno

   1. Duplica el archivo .env.example y renómbralo como .env.local:

   ```bash
   cp .env.example .env.local
   ```

   2. Llena los valores correspondientes con la configuración de tu proyecto de Firebase:

   ```env
   VITE_FIREBASE_API_KEY=TU_API_KEY
   VITE_FIREBASE_AUTH_DOMAIN=TU_PROYECTO.firebaseapp.com
   VITE_FIREBASE_PROJECT_ID=TU_PROJECT_ID
   VITE_FIREBASE_STORAGE_BUCKET=TU_PROYECTO.appspot.com
   VITE_FIREBASE_MESSAGING_SENDER_ID=NUMERO_SENDER_ID
   VITE_FIREBASE_APP_ID=TU_APP_ID
   ```

   > Puedes encontrar estos datos en la consola de Firebase en la sección `Configuración del proyecto > General`.

4. Ejecuta el proyecto:
   ```bash
   yarn dev
   ```

---

## 🔧 Screenshots (próximamente)

> Se incluirán capturas del dashboard de representantes y administradores.

---

## 📦 Deployment

Puedes desplegarlo fácilmente en:

- [Vercel](https://vercel.com/)
- [Netlify](https://www.netlify.com/)
- [Firebase Hosting](https://firebase.google.com/products/hosting)

---
