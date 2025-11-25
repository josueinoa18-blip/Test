Xclusive Price Finder - Proyecto completo (MVP)
Contenido:
- backend/: Express API (server.js) con endpoints básicos (search, product, admin offers, Stripe checkout stub)
- frontend/: Next.js App Router (src/app) con páginas: page.js, product/[id]/page.js, cart/page.js, admin basic
- scraper/: ejemplo simple de scraper en Python (educativo)
- db/: esquema SQL para Postgres
- demo-static/: Página HTML/CSS/JS que muestra una demo rápida (sin backend) para ver UI inmediatamente

Instrucciones rápidas (preview local estático):
1) Extrae el zip y abre demo-static/demo.html en tu navegador para ver una demo visual rápida sin backend.
2) Para correr en local (completo):
   - Requiere Node.js (>=18), npm, PostgreSQL y (opcional) Stripe keys para pagos.
   - Backend:
     cd backend
     npm install
     Ajusta DATABASE_URL en .env si usas Postgres. Luego:
     node server.js
     (API correrá en http://localhost:4000)
   - Frontend:
     cd frontend
     npm install
     npm run dev
     (Next.js correrá en http://localhost:3000)
3) Ejecución del scraper (educativo):
   cd scraper
   pip install -r requirements.txt
   Ajusta conexión a Postgres y ejecuta
   python scraper_worker.py

Nota: Los valores de Stripe son placeholders (pk_test_XXXX, sk_test_XXXX). Reemplaza por tus claves de prueba.
Seguridad/legal: Respeta TOS de sitios y robots.txt; usa APIs oficiales cuando sea posible.
