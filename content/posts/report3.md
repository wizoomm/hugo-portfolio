---
title: "Работа с фреймворком Bootstrap 5"
date: 2025-09-20
draft: false
---

Картинку для сайта брала на [PrimeCamper.ru](https://primecamper.ru)

Ссылка на мой [kodaktor](https://kodaktor.ru/g/5a4efde)

**Код страницы, написанный на сайте kodaktor.ru**
```html
<!doctype html>
<html lang="ru">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Volkswagen Grand California — лендинг на Bootstrap 5</title>


  <link
    href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css"
    rel="stylesheet"
  >


  <link
    href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.2/css/all.min.css"
    rel="stylesheet"
  />

  <style>
    body { padding-top: 4.5rem; }
    .lead { color: #555; }

    .feature-icon {
      font-size: 2.2rem;
      line-height: 1;
      color: #000; 
    }

    h1, h2, h3 { letter-spacing: .2px; }
    footer { background: #f8f9fa; }
  </style>
</head>
<body>


  <nav class="navbar navbar-expand-lg bg-white border-bottom fixed-top">
    <div class="container">
      <a class="navbar-brand fw-semibold" href="#">
        <i class="fa-solid fa-van-shuttle me-2 feature-icon"></i>Grand California
      </a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#mainNav">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="mainNav">
        <ul class="navbar-nav ms-auto">
          <li class="nav-item"><a class="nav-link active" href="#hero">Главная</a></li>
          <li class="nav-item"><a class="nav-link" href="#contacts">Контакты</a></li>
        </ul>
      </div>
    </div>
  </nav>

  <section id="hero" class="py-5 bg-light">
    <div class="container py-4">
      <div class="row align-items-center g-4">
        <div class="col-12 col-lg-7">
          <h1 class="display-5 fw-bold">Добро пожаловать!</h1>
          <h2 class="h4 text-secondary mt-3">
            Комфортный автодом на базе <span class="fw-semibold">Volkswagen Grand California</span>.
          </h2>
          <p class="lead mt-3">Просторный интерьер, спальные места, кухня, душ — всё, чтобы чувствовать себя как дома.</p>
          <div class="d-flex gap-3 mt-4">
            <!-- теперь кнопка чёрная -->
            <a href="#features" class="btn btn-dark btn-lg">Узнать больше</a>
            <button class="btn btn-outline-secondary btn-lg" data-bs-toggle="modal" data-bs-target="#contactModal">
              Написать нам
            </button>
          </div>
        </div>
        <div class="col-12 col-lg-5 text-center">
          <img src="https://primecamper.ru/assets/cache_image/products/68/whatsapp-image-2023-07-01-at-17.31.23_0x0_28d.jpeg" 
               class="img-fluid rounded shadow-sm" alt="Volkswagen Grand California">
        </div>
      </div>
    </div>
  </section>


  <section id="features" class="py-5">
    <div class="container">
      <div class="text-center mb-5">
        <h3 class="fw-bold">Почему это удобно</h3>
        <p class="text-secondary mb-0">Три ключевые причины выбрать Grand California</p>
      </div>

      <div class="row g-4">
        <div class="col-12 col-lg-4 order-2 order-lg-1">
          <div class="card h-100 shadow-sm">
            <div class="card-body d-flex gap-3 align-items-start">
              <i class="fa-solid fa-campground feature-icon"></i>
              <div>
                <h5 class="card-title mb-2">Свобода маршрута</h5>
                <p class="card-text mb-0">Езжай куда хочешь и останавливайся где удобно.</p>
              </div>
            </div>
          </div>
        </div>

        <div class="col-12 col-lg-4 order-1 order-lg-2">
          <div class="card h-100 shadow-sm">
            <div class="card-body d-flex gap-3 align-items-start">
              <i class="fa-solid fa-shower feature-icon"></i>
              <div>
                <h5 class="card-title mb-2">Комфорт как дома</h5>
                <p class="card-text mb-0">Душ, удобные кровати, кухня — путешествия без компромиссов.</p>
              </div>
            </div>
          </div>
        </div>

        <div class="col-12 col-lg-4 order-3 order-lg-3">
          <div class="card h-100 shadow-sm">
            <div class="card-body d-flex gap-3 align-items-start">
              <i class="fa-solid fa-solar-panel feature-icon"></i>
              <div>
                <h5 class="card-title mb-2">Автономия</h5>
                <p class="card-text mb-0">Современные системы питания обеспечивают независимость.</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>


  <footer id="contacts" class="py-4 d-none d-md-block">
    <div class="container">
      <div class="row g-3 align-items-center">
        <div class="col-md"><span class="text-secondary small">Телефон</span><div class="fw-medium">+7 (921) 753-66-83</div></div>
        <div class="col-md"><span class="text-secondary small">Email</span><div class="fw-medium">grandcalifornia@gmail.com</div></div>
        <div class="col-md"><span class="text-secondary small">Адрес</span><div class="fw-medium">Москва, Солнечная ул., 1</div></div>
        
    </div>
  </footer>


  <div class="modal fade" id="contactModal" tabindex="-1">
    <div class="modal-dialog modal-dialog-centered">
      <div class="modal-content">
        <form class="needs-validation" novalidate>
          <div class="modal-header">
            <h5 class="modal-title">Связаться с нами</h5>
            <button type="button" class="btn-close" data-bs-dismiss="modal"></button>
          </div>
          <div class="modal-body">
            <div class="mb-3">
              <label for="name" class="form-label">Имя</label>
              <input type="text" class="form-control" id="name" required>
              <div class="invalid-feedback">Введите имя.</div>
            </div>
            <div class="mb-3">
              <label for="email" class="form-label">Email</label>
              <input type="email" class="form-control" id="email" required>
              <div class="invalid-feedback">Укажите корректный email.</div>
            </div>
            <div class="mb-3">
              <label for="message" class="form-label">Сообщение</label>
              <textarea class="form-control" id="message" rows="4" required></textarea>
              <div class="invalid-feedback">Напишите сообщение.</div>
            </div>
          </div>
          <div class="modal-footer">
            <button type="submit" class="btn btn-primary w-100">Отправить</button>
          </div>
        </form>
      </div>
    </div>
  </div>


  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>

  <script>
    (() => {
      'use strict';
      const forms = document.querySelectorAll('.needs-validation');
      Array.from(forms).forEach(form => {
        form.addEventListener('submit', event => {
          if (!form.checkValidity()) {
            event.preventDefault();
            event.stopPropagation();
          } else {
            event.preventDefault();
            const modalEl = document.getElementById('contactModal');
            const modal = bootstrap.Modal.getInstance(modalEl);
            modal.hide();
            alert('Спасибо! Мы скоро свяжемся с вами.');
            form.reset();
          }
          form.classList.add('was-validated');
        }, false);
      });
    })();
  </script>
</body>
</html>
```
