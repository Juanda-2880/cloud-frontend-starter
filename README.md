# ☁️ Cloud Frontend Starter

![Status](https://img.shields.io/badge/Status-Completed-success)
![AWS S3](https://img.shields.io/badge/AWS-S3-orange?logo=amazon-aws)
![Cloudflare](https://img.shields.io/badge/Cloudflare-DNS%20%26%20SSL-f38020?logo=cloudflare)
![License](https://img.shields.io/badge/License-MIT-blue)

Una arquitectura de referencia para desplegar aplicaciones web estáticas (React, Vue, HTML/CSS) utilizando **AWS S3** para el alojamiento y **Cloudflare** para la gestión de DNS y seguridad SSL.

Este proyecto demuestra cómo lograr un despliegue de alto rendimiento, globalmente distribuido y seguro, manteniendo una estrategia de **costo cero (o casi cero)** para entornos de desarrollo y práctica.

---

## 📖 Tabla de Contenidos
- [El Problema y la Solución](#-el-problema-y-la-solución)
- [Arquitectura](#-arquitectura)
- [Tecnologías Usadas](#-tecnologías-usadas)
- [Guía de Despliegue](#-guía-de-despliegue)
- [Configuración de DNS (El "Truco" de Costos)](#-configuración-de-dns-el-truco-de-costos)
- [Estructura del Proyecto](#-estructura-del-proyecto)
- [Próximos Pasos](#-próximos-pasos)
- [Autor](#-autor)

---

## 💡 El Problema y la Solución

### El Reto
Desplegar una aplicación frontend en AWS tradicionalmente implica usar **S3** (almacenamiento) + **Route 53** (DNS) + **CloudFront** (CDN/SSL). Sin embargo, Route 53 no tiene capa gratuita (costo fijo de $0.50/mes por zona) y la configuración de certificados SSL en AWS puede ser compleja para proyectos pequeños.

### La Solución Propuesta
Esta arquitectura desacopla la capa de DNS y CDN de AWS, delegándola a **Cloudflare**.

* **Ahorro de Costos:** Se elimina el costo de la Hosted Zone de Route 53.
* **Seguridad:** Obtenemos SSL (HTTPS) automático y gratuito gestionado por Cloudflare (AWS S3 hosting estático solo ofrece HTTP nativamente).
* **Simplicidad:** Gestión de DNS simplificada y propagación rápida.

