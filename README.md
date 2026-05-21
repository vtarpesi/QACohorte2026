README — Cypress QA Automation (Technology with Purpose by Santex) 🚀🧪

Descripción

Repositorio para almacenar ejercicios, ejemplos y buenas prácticas en Cypress orientadas a QA Automation. 🎯
Objetivo: aprender y documentar lo relevante de automatización de pruebas (end-to-end, integración, componentes) siguiendo la filosofía Technology with Purpose de Santex. 💡🤝
Contenido del repositorio

/cypress
/e2e — pruebas end-to-end (tests, fixtures, commands) 🖥️
/integration — ejemplos históricos o alternativos (si aplicable) 🔁
/component — pruebas de componentes (si se usa) 🧩
/support — comandos personalizados, hooks, configuración global ⚙️
/fixtures — datos de prueba reutilizables 📂
cypress.config.js — configuración principal de Cypress 🛠️
package.json — dependencias y scripts 📦
README.md — este archivo 📘
/docs — guías, notas de aprendizaje, referencias 📚
/examples — proyectos o casos de prueba completos de referencia 🧾
Instalación (asumiendo Node.js >= 16) 🧰

Clonar el repositorio: git clone ⤵️
Entrar al directorio: cd 📁
Instalar dependencias: npm install ⚡
Scripts útiles (package.json) ▶️

npm run cypress:open — abrir la UI interactiva de Cypress 🖱️
npm run cypress:run — ejecutar tests en modo headless 🏃‍♀️
npm run lint — (si aplica) correr linter 🧹
npm run test:ci — (si aplica) ejecutar suite en CI 🧑‍💻
Estructura de ejemplo de un test (resumen) 🧭

Usa describe/it para agrupar casos. 🗂️
Antes: cy.visit(), cy.intercept() para stubs/mocks. 🔌
Comandos recomendados: cy.get(), cy.contains(), cy.click(), cy.type(), cy.should(). ✋
Separar selectores en data-* attributes (p. ej. data-cy) para mantener pruebas robustas. 🏷️
Buenas prácticas ✅

Usar selectores estables (data-attributes) en lugar de selectores de presentación. 🔒
Mantener tests pequeños y deterministas. 🧩
Limpiar estado entre pruebas (API calls para reset, o uso de fixtures). 🧼
Evitar dependencias entre tests; cada prueba debe poder ejecutarse aislada. 🚪
Mockear llamadas externas cuando sea necesario para evitar flakiness. 🎭
Añadir timeouts razonables y esperar por condiciones en vez de sleeps fijos. ⏳
Componer comandos personalizados en cypress/support/commands.js para reutilización. ♻️
Versionar fixtures y mantener datos de prueba pequeños y representativos. 🗃️
Integración con CI 🤖

Configurar un job que instale dependencias y ejecute: npm ci
npm run cypress:run
Usar contenedores o runners que soporten navegadores (o Cypress Dashboard si aplica). 🐳
Guardar artefactos: videos, screenshots y reportes de resultados. 📸🎥
Reporting y debugging 🔍

Habilitar screenshots y videos en cypress.config.js para fallos. 📷
Usar mochawesome, junit u otros reporters si necesitas integrarlo con CI. 🧾
Reproducir fallos localmente con npm run cypress:open y el spec fallido. 🛠️
Ejemplos de casos de uso a incluir 📝

Login exitoso y fallido. 🔐
Flujo de compra/carrito. 🛒
Formularios con validaciones y mensajes de error. 🧾
Pruebas de accesibilidad básicas (axe-core). ♿
Pruebas con datos parametrizados (fixtures). 🔁
Tests de API (cy.request) para validación rápida de backend. 🔗
Convenciones del repositorio 🌿

Branch main: código establecido y estable. ✅
Branch feature/- para trabajo en curso. ✨
PRs con descripción, pasos para reproducir y capturas si aplica. 📌
Issues etiquetados: bug, enhancement, docs, flaky. 🏷️
Recursos y referencias 📚

Documentación oficial de Cypress (añadir link en /docs si se quiere). 🔗
Guías internas Santex sobre "Technology with Purpose" (mencionar ubicación en /docs). 🧭
Cómo contribuir 🤝

Abrir un issue proponiendo la mejora o ejercicio. 🗣️
Crear una branch feature/ con cambios. 🌱
Hacer PR describiendo objetivo y pruebas realizadas. 📬
Mantener commits pequeños y claros. ✍️
Licencia 📜

Añadir la licencia que prefieras (MIT, Apache-2.0, etc.). Recomiendo MIT para fines educativos. 🏷️
Contacto 📬

Incluir maintainer o equipo de Santex (correo o handle) en /MAINTAINERS (opcional). 👥
Fecha 🗓️

Última actualización: 21 de mayo de 202*
