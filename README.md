<!DOCTYPE html>
<html lang="es">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>3D Prints Elegance - Impresiones 3D Personalizadas</title>
    <script src="https://cdn.tailwindcss.com/3.4.16"></script>
    <script>
      tailwind.config = {
        theme: {
          extend: {
            colors: { primary: "#D4AF37", secondary: "#F5F5F5" },
            borderRadius: {
              none: "0px",
              sm: "4px",
              DEFAULT: "8px",
              md: "12px",
              lg: "16px",
              xl: "20px",
              "2xl": "24px",
              "3xl": "32px",
              full: "9999px",
              button: "8px",
            },
          },
        },
      };
    </script>
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Pacifico&display=swap"
      rel="stylesheet"
    />
    <link
      href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@400;500;600;700&family=Montserrat:wght@300;400;500;600&display=swap"
      rel="stylesheet"
    />
    <link
      href="https://cdn.jsdelivr.net/npm/remixicon@4.5.0/fonts/remixicon.css"
      rel="stylesheet"
    />
    <style>
      :where([class^="ri-"])::before { content: "\f3c2"; }
      body {
          font-family: 'Montserrat', sans-serif;
          color: #333;
      }
      h1, h2, h3, h4, h5, h6 {
          font-family: 'Cormorant Garamond', serif;
      }
      .hero-section {
          background-image: url('https://public.readdy.ai/ai/img_res/3a17f19c744c55d5795a31df32084123.jpg');
          background-size: cover;
          background-position: center;
      }
      .nav-link {
          position: relative;
      }
      .nav-link::after {
          content: '';
          position: absolute;
          width: 0;
          height: 1px;
          bottom: -2px;
          left: 0;
          background-color: #D4AF37;
          transition: width 0.3s ease;
      }
      .nav-link:hover::after {
          width: 100%;
      }
      input[type="number"]::-webkit-inner-spin-button,
      input[type="number"]::-webkit-outer-spin-button {
          -webkit-appearance: none;
          margin: 0;
      }
      .category-card {
          transition: all 0.3s ease;
      }
      .category-card:hover {
          transform: translateY(-5px);
          box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
      }
      .timeline-item {
          position: relative;
      }
      .timeline-item::after {
          content: '';
          position: absolute;
          top: 50%;
          right: -50px;
          width: 50px;
          height: 1px;
          background-color: #D4AF37;
      }
      .timeline-item:last-child::after {
          display: none;
      }
      .gallery-item {
          transition: all 0.3s ease;
      }
      .gallery-item:hover .overlay {
          opacity: 1;
      }
    </style>
  </head>
  <body class="bg-white min-h-screen">
    <!-- Navegación -->
    <header class="bg-secondary sticky top-0 z-50 shadow-sm">
      <div
        class="container mx-auto px-4 py-4 flex justify-between items-center"
      >
        <div class="w-36 text-center">
          <h1 class="font-['Pacifico'] text-3xl text-primary">logo</h1>
        </div>

        <nav class="hidden md:flex space-x-8">
          <a
            href="#llaveros"
            class="nav-link text-gray-800 hover:text-primary transition-colors"
            >Llaveros</a
          >
          <a
            href="#gaming"
            class="nav-link text-gray-800 hover:text-primary transition-colors"
            >Gaming</a
          >
          <a
            href="#figuras"
            class="nav-link text-gray-800 hover:text-primary transition-colors"
            >Figuras</a
          >
          <a
            href="#bustos"
            class="nav-link text-gray-800 hover:text-primary transition-colors"
            >Bustos</a
          >
          <a
            href="#personalizados"
            class="nav-link text-gray-800 hover:text-primary transition-colors"
            >Personalizados</a
          >
        </nav>

        <div class="md:hidden w-10 h-10 flex items-center justify-center">
          <button class="text-gray-800" id="mobile-menu-button">
            <i class="ri-menu-line ri-lg"></i>
          </button>
        </div>
      </div>

      <!-- Menú móvil -->
      <div
        class="md:hidden hidden bg-white absolute w-full shadow-md"
        id="mobile-menu"
      >
        <div class="container mx-auto px-4 py-2 flex flex-col space-y-3">
          <a
            href="#llaveros"
            class="py-2 text-gray-800 hover:text-primary transition-colors"
            >Llaveros</a
          >
          <a
            href="#gaming"
            class="py-2 text-gray-800 hover:text-primary transition-colors"
            >Gaming</a
          >
          <a
            href="#figuras"
            class="py-2 text-gray-800 hover:text-primary transition-colors"
            >Figuras</a
          >
          <a
            href="#bustos"
            class="py-2 text-gray-800 hover:text-primary transition-colors"
            >Bustos</a
          >
          <a
            href="#personalizados"
            class="py-2 text-gray-800 hover:text-primary transition-colors"
            >Personalizados</a
          >
        </div>
      </div>
    </header>

    <!-- Hero Section -->
    <section class="hero-section relative">
      <div class="absolute inset-0 bg-black bg-opacity-20"></div>
      <div class="container mx-auto px-4 py-24 md:py-32 relative z-10">
        <div class="max-w-2xl">
          <h1
            class="text-4xl md:text-5xl lg:text-6xl font-bold text-white mb-4"
          >
            Arte en 3D Personalizado
          </h1>
          <p class="text-xl md:text-2xl text-white mb-8">
            Creaciones únicas diseñadas para ti. Desde llaveros hasta figuras
            detalladas, hacemos realidad tus ideas.
          </p>
          <a
            href="https://instagram.com/username"
            target="_blank"
            class="inline-flex items-center bg-primary text-white px-6 py-3 rounded-button hover:bg-opacity-90 transition-all shadow-lg whitespace-nowrap"
          >
            <span class="w-6 h-6 flex items-center justify-center mr-2">
              <i class="ri-instagram-line"></i>
            </span>
            Contactar por Instagram
          </a>
        </div>
      </div>
    </section>
    <!-- Categorías Principales -->
    <section class="py-16 bg-white">
      <div class="container mx-auto px-4">
        <h2 class="text-3xl md:text-4xl font-semibold text-center mb-12">
          Nuestras Categorías
        </h2>

        <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
          <!-- Categoría 1: Llaveros -->
          <div
            id="llaveros"
            class="category-card bg-secondary rounded border border-gray-200 overflow-hidden group"
          >
            <div class="h-64 overflow-hidden">
              <img
                src="https://public.readdy.ai/ai/img_res/daa0fee20f952bb9dcda9f7638371f2c.jpg"
                alt="Llaveros personalizados"
                class="w-full h-full object-cover object-top transition-transform duration-500 group-hover:scale-105"
              />
            </div>
            <div class="p-6 border-t border-primary">
              <h3 class="text-2xl font-semibold mb-3">Llaveros</h3>
              <p class="text-gray-700 mb-4">
                Llaveros personalizados con diseños únicos. Elige colores,
                formas y tamaños para crear un accesorio que refleje tu
                personalidad.
              </p>
              <a href="#" class="text-primary font-medium flex items-center">
                Ver colección
                <span class="w-5 h-5 flex items-center justify-center ml-1">
                  <i class="ri-arrow-right-line"></i>
                </span>
              </a>
            </div>
          </div>

          <!-- Categoría 2: Gaming -->
          <div
            id="gaming"
            class="category-card bg-secondary rounded border border-gray-200 overflow-hidden group"
          >
            <div class="h-64 overflow-hidden">
              <img
                src="https://public.readdy.ai/ai/img_res/fae36e16099111b474b4ee95eabbe951.jpg"
                alt="Accesorios gaming"
                class="w-full h-full object-cover object-top transition-transform duration-500 group-hover:scale-105"
              />
            </div>
            <div class="p-6 border-t border-primary">
              <h3 class="text-2xl font-semibold mb-3">Gaming</h3>
              <p class="text-gray-700 mb-4">
                Soportes para auriculares, mandos y accesorios gaming que
                combinan funcionalidad con estilo. Mejora tu setup con diseños
                exclusivos.
              </p>
              <a href="#" class="text-primary font-medium flex items-center">
                Ver colección
                <span class="w-5 h-5 flex items-center justify-center ml-1">
                  <i class="ri-arrow-right-line"></i>
                </span>
              </a>
            </div>
          </div>

          <!-- Categoría 3: Figuras y Bustos -->
          <div
            id="figuras"
            class="category-card bg-secondary rounded border border-gray-200 overflow-hidden group"
          >
            <div class="h-64 overflow-hidden">
              <img
                src="https://public.readdy.ai/ai/img_res/ad7ce30b5f592579cc778e3e8947c517.jpg"
                alt="Figuras y bustos"
                class="w-full h-full object-cover object-top transition-transform duration-500 group-hover:scale-105"
              />
            </div>
            <div class="p-6 border-t border-primary">
              <h3 class="text-2xl font-semibold mb-3">Figuras y Bustos</h3>
              <p class="text-gray-700 mb-4">
                Figuras detalladas y bustos personalizados. Desde personajes de
                ficción hasta retratos realistas, creamos piezas únicas con gran
                detalle.
              </p>
              <a href="#" class="text-primary font-medium flex items-center">
                Ver colección
                <span class="w-5 h-5 flex items-center justify-center ml-1">
                  <i class="ri-arrow-right-line"></i>
                </span>
              </a>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Sección de Personalizados -->
    <section id="personalizados" class="py-16 bg-gray-50">
      <div class="container mx-auto px-4">
        <h2 class="text-3xl md:text-4xl font-semibold text-center mb-4">
          Diseños Personalizados
        </h2>
        <p class="text-gray-700 text-center max-w-3xl mx-auto mb-12">
          Si puedes imaginarlo, podemos crearlo. Nuestro servicio de diseños
          personalizados te permite convertir cualquier idea en una pieza única
          impresa en 3D.
        </p>

        <!-- Filtros -->
        <div class="flex flex-wrap justify-center gap-4 mb-10">
          <button
            class="px-6 py-2 bg-white border border-gray-300 rounded-full hover:border-primary hover:text-primary transition-colors focus:outline-none focus:ring-2 focus:ring-primary focus:ring-opacity-50 active whitespace-nowrap"
          >
            Todos
          </button>
          <button
            class="px-6 py-2 bg-white border border-gray-300 rounded-full hover:border-primary hover:text-primary transition-colors focus:outline-none whitespace-nowrap"
          >
            Llaveros
          </button>
          <button
            class="px-6 py-2 bg-white border border-gray-300 rounded-full hover:border-primary hover:text-primary transition-colors focus:outline-none whitespace-nowrap"
          >
            Gaming
          </button>
          <button
            class="px-6 py-2 bg-white border border-gray-300 rounded-full hover:border-primary hover:text-primary transition-colors focus:outline-none whitespace-nowrap"
          >
            Figuras
          </button>
          <button
            class="px-6 py-2 bg-white border border-gray-300 rounded-full hover:border-primary hover:text-primary transition-colors focus:outline-none whitespace-nowrap"
          >
            Bustos
          </button>
        </div>

        <!-- Galería -->
        <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6">
          <!-- Galería Item 1 -->
          <div class="gallery-item relative rounded overflow-hidden group">
            <img
              src="https://public.readdy.ai/ai/img_res/c6f9c726e8d04f1fb14cae1c35650d81.jpg"
              alt="Llavero personalizado"
              class="w-full h-72 object-cover object-top"
            />
            <div
              class="overlay absolute inset-0 bg-black bg-opacity-50 flex flex-col justify-end p-6 opacity-0 transition-opacity"
            >
              <h3 class="text-white text-xl font-semibold">
                Llavero Personalizado
              </h3>
              <p class="text-gray-200 mb-4">
                Diseño exclusivo con nombre grabado
              </p>
            </div>
          </div>

          <!-- Galería Item 2 -->
          <div class="gallery-item relative rounded overflow-hidden group">
            <img
              src="https://public.readdy.ai/ai/img_res/6819c75dbf1018cacdaeb4282a44be0b.jpg"
              alt="Soporte para auriculares"
              class="w-full h-72 object-cover object-top"
            />
            <div
              class="overlay absolute inset-0 bg-black bg-opacity-50 flex flex-col justify-end p-6 opacity-0 transition-opacity"
            >
              <h3 class="text-white text-xl font-semibold">
                Soporte para Auriculares
              </h3>
              <p class="text-gray-200 mb-4">
                Diseño ergonómico con temática gaming
              </p>
            </div>
          </div>

          <!-- Galería Item 3 -->
          <div class="gallery-item relative rounded overflow-hidden group">
            <img
              src="https://public.readdy.ai/ai/img_res/139777a6e58aebc3b14aa5b7bee6353b.jpg"
              alt="Figura de personaje"
              class="w-full h-72 object-cover object-top"
            />
            <div
              class="overlay absolute inset-0 bg-black bg-opacity-50 flex flex-col justify-end p-6 opacity-0 transition-opacity"
            >
              <h3 class="text-white text-xl font-semibold">
                Figura de Personaje
              </h3>
              <p class="text-gray-200 mb-4">
                Recreación detallada de personaje de videojuego
              </p>
            </div>
          </div>

          <!-- Galería Item 4 -->
          <div class="gallery-item relative rounded overflow-hidden group">
            <img
              src="https://public.readdy.ai/ai/img_res/2483e0938fd04883aebcd680707cc826.jpg"
              alt="Soporte para mando"
              class="w-full h-72 object-cover object-top"
            />
            <div
              class="overlay absolute inset-0 bg-black bg-opacity-50 flex flex-col justify-end p-6 opacity-0 transition-opacity"
            >
              <h3 class="text-white text-xl font-semibold">
                Soporte para Mando
              </h3>
              <p class="text-gray-200 mb-4">
                Base elegante con capacidad de carga
              </p>
            </div>
          </div>

          <!-- Galería Item 5 -->
          <div class="gallery-item relative rounded overflow-hidden group">
            <img
              src="https://public.readdy.ai/ai/img_res/43b7656d662f354cff17a34c66d1f99b.jpg"
              alt="Busto personalizado"
              class="w-full h-72 object-cover object-top"
            />
            <div
              class="overlay absolute inset-0 bg-black bg-opacity-50 flex flex-col justify-end p-6 opacity-0 transition-opacity"
            >
              <h3 class="text-white text-xl font-semibold">
                Busto Personalizado
              </h3>
              <p class="text-gray-200 mb-4">
                Retrato 3D con gran nivel de detalle
              </p>
            </div>
          </div>

          <!-- Galería Item 6 -->
          <div class="gallery-item relative rounded overflow-hidden group">
            <img
              src="https://public.readdy.ai/ai/img_res/36c50036b6a3d7bfcd28c678f02d7cdd.jpg"
              alt="Pieza decorativa"
              class="w-full h-72 object-cover object-top"
            />
            <div
              class="overlay absolute inset-0 bg-black bg-opacity-50 flex flex-col justify-end p-6 opacity-0 transition-opacity"
            >
              <h3 class="text-white text-xl font-semibold">Pieza Decorativa</h3>
              <p class="text-gray-200 mb-4">
                Elemento arquitectónico para decoración
              </p>
            </div>
          </div>
        </div>

        <!-- CTA -->
        <div class="text-center mt-12">
          <a
            href="https://instagram.com/username"
            target="_blank"
            class="inline-flex items-center bg-primary text-white px-8 py-3 rounded-button hover:bg-opacity-90 transition-all shadow-lg whitespace-nowrap"
          >
            <span class="w-6 h-6 flex items-center justify-center mr-2">
              <i class="ri-message-3-line"></i>
            </span>
            Solicitar Diseño Personalizado
          </a>
        </div>
      </div>
    </section>

    <!-- Proceso de Trabajo -->
    <section class="py-16 bg-white">
      <div class="container mx-auto px-4">
        <h2 class="text-3xl md:text-4xl font-semibold text-center mb-12">
          Nuestro Proceso
        </h2>

        <div
          class="flex flex-col md:flex-row justify-between items-start md:items-center gap-8 md:gap-4"
        >
          <!-- Paso 1 -->
          <div
            class="timeline-item flex flex-col items-center text-center max-w-xs mx-auto"
          >
            <div
              class="w-20 h-20 flex items-center justify-center bg-secondary rounded-full border-2 border-primary mb-4"
            >
              <i class="ri-pencil-ruler-2-line ri-2x text-primary"></i>
            </div>
            <h3 class="text-xl font-semibold mb-2">Diseño</h3>
            <p class="text-gray-700">
              Conversamos sobre tu idea y creamos un diseño digital
              personalizado.
            </p>
          </div>

          <!-- Paso 2 -->
          <div
            class="timeline-item flex flex-col items-center text-center max-w-xs mx-auto"
          >
            <div
              class="w-20 h-20 flex items-center justify-center bg-secondary rounded-full border-2 border-primary mb-4"
            >
              <i class="ri-check-double-line ri-2x text-primary"></i>
            </div>
            <h3 class="text-xl font-semibold mb-2">Aprobación</h3>
            <p class="text-gray-700">
              Te enviamos una vista previa para tu aprobación antes de imprimir.
            </p>
          </div>

          <!-- Paso 3 -->
          <div
            class="timeline-item flex flex-col items-center text-center max-w-xs mx-auto"
          >
            <div
              class="w-20 h-20 flex items-center justify-center bg-secondary rounded-full border-2 border-primary mb-4"
            >
              <i class="ri-printer-line ri-2x text-primary"></i>
            </div>
            <h3 class="text-xl font-semibold mb-2">Impresión</h3>
            <p class="text-gray-700">
              Imprimimos tu diseño con materiales de alta calidad y precisión.
            </p>
          </div>

          <!-- Paso 4 -->
          <div
            class="timeline-item flex flex-col items-center text-center max-w-xs mx-auto"
          >
            <div
              class="w-20 h-20 flex items-center justify-center bg-secondary rounded-full border-2 border-primary mb-4"
            >
              <i class="ri-gift-line ri-2x text-primary"></i>
            </div>
            <h3 class="text-xl font-semibold mb-2">Entrega</h3>
            <p class="text-gray-700">
              Empaquetamos cuidadosamente y enviamos tu creación personalizada.
            </p>
          </div>
        </div>
      </div>
    </section>

    <!-- Testimonios -->
    <section class="py-16 bg-gray-50">
      <div class="container mx-auto px-4">
        <h2 class="text-3xl md:text-4xl font-semibold text-center mb-12">
          Lo Que Dicen Nuestros Clientes
        </h2>

        <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
          <!-- Testimonio 1 -->
          <div class="bg-white p-6 rounded shadow-sm border border-gray-100">
            <div class="flex items-center mb-4">
              <div class="text-primary">
                <i class="ri-star-fill"></i>
                <i class="ri-star-fill"></i>
                <i class="ri-star-fill"></i>
                <i class="ri-star-fill"></i>
                <i class="ri-star-fill"></i>
              </div>
            </div>
            <p class="text-gray-700 mb-4">
              "Encargué un llavero personalizado con el nombre de mi hijo y
              quedó perfecto. La calidad es excelente y el servicio muy atento.
              Volveré a comprar sin duda."
            </p>
            <div class="font-semibold">Martina Rodríguez</div>
          </div>

          <!-- Testimonio 2 -->
          <div class="bg-white p-6 rounded shadow-sm border border-gray-100">
            <div class="flex items-center mb-4">
              <div class="text-primary">
                <i class="ri-star-fill"></i>
                <i class="ri-star-fill"></i>
                <i class="ri-star-fill"></i>
                <i class="ri-star-fill"></i>
                <i class="ri-star-fill"></i>
              </div>
            </div>
            <p class="text-gray-700 mb-4">
              "El soporte para auriculares que diseñaron para mi setup gaming es
              increíble. Combina perfectamente con mi decoración y es muy
              funcional. Gracias por el gran trabajo."
            </p>
            <div class="font-semibold">Carlos Mendoza</div>
          </div>

          <!-- Testimonio 3 -->
          <div class="bg-white p-6 rounded shadow-sm border border-gray-100">
            <div class="flex items-center mb-4">
              <div class="text-primary">
                <i class="ri-star-fill"></i>
                <i class="ri-star-fill"></i>
                <i class="ri-star-fill"></i>
                <i class="ri-star-fill"></i>
                <i class="ri-star-fill"></i>
              </div>
            </div>
            <p class="text-gray-700 mb-4">
              "Pedí una figura personalizada de mi personaje favorito de
              videojuegos y el resultado superó mis expectativas. El nivel de
              detalle es impresionante. Totalmente recomendado."
            </p>
            <div class="font-semibold">Laura Fernández</div>
          </div>
        </div>
      </div>
    </section>
    <!-- Contacto -->
    <section class="py-16 bg-white">
      <div class="container mx-auto px-4">
        <div
          class="max-w-4xl mx-auto bg-secondary rounded-lg p-8 md:p-12 shadow-sm"
        >
          <h2 class="text-3xl md:text-4xl font-semibold text-center mb-6">
            ¿Listo para Tu Diseño Personalizado?
          </h2>
          <p class="text-gray-700 text-center mb-8">
            Contacta con nosotros a través de Instagram y cuéntanos tu idea.
            Estaremos encantados de ayudarte a hacerla realidad.
          </p>

          <div class="flex flex-col sm:flex-row justify-center gap-4">
            <a
              href="https://instagram.com/username"
              target="_blank"
              class="inline-flex items-center justify-center bg-primary text-white px-8 py-3 rounded-button hover:bg-opacity-90 transition-all shadow-lg whitespace-nowrap"
            >
              <span class="w-6 h-6 flex items-center justify-center mr-2">
                <i class="ri-instagram-line"></i>
              </span>
              Contactar por Instagram
            </a>

            <a
              href="mailto:info@ejemplo.com"
              class="inline-flex items-center justify-center bg-white text-gray-800 border border-gray-300 px-8 py-3 rounded-button hover:border-primary hover:text-primary transition-all whitespace-nowrap"
            >
              <span class="w-6 h-6 flex items-center justify-center mr-2">
                <i class="ri-mail-line"></i>
              </span>
              Enviar Email
            </a>
          </div>
        </div>
      </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-900 text-white py-12">
      <div class="container mx-auto px-4">
        <div class="grid grid-cols-1 md:grid-cols-4 gap-8">
          <!-- Logo y descripción -->
          <div class="md:col-span-2">
            <h1 class="font-['Pacifico'] text-3xl text-primary mb-4">logo</h1>
            <p class="text-gray-400 mb-6">
              Creaciones únicas en impresión 3D. Diseños personalizados que dan
              vida a tus ideas con calidad y atención al detalle.
            </p>
            <div class="flex space-x-4">
              <a
                href="#"
                class="w-10 h-10 flex items-center justify-center bg-gray-800 rounded-full hover:bg-primary transition-colors"
              >
                <i class="ri-instagram-line"></i>
              </a>
              <a
                href="#"
                class="w-10 h-10 flex items-center justify-center bg-gray-800 rounded-full hover:bg-primary transition-colors"
              >
                <i class="ri-facebook-line"></i>
              </a>
              <a
                href="#"
                class="w-10 h-10 flex items-center justify-center bg-gray-800 rounded-full hover:bg-primary transition-colors"
              >
                <i class="ri-whatsapp-line"></i>
              </a>
            </div>
          </div>

          <!-- Enlaces rápidos -->
          <div>
            <h3 class="text-lg font-semibold mb-4 border-b border-primary pb-2">
              Enlaces Rápidos
            </h3>
            <ul class="space-y-2">
              <li>
                <a
                  href="#llaveros"
                  class="text-gray-400 hover:text-primary transition-colors"
                  >Llaveros</a
                >
              </li>
              <li>
                <a
                  href="#gaming"
                  class="text-gray-400 hover:text-primary transition-colors"
                  >Gaming</a
                >
              </li>
              <li>
                <a
                  href="#figuras"
                  class="text-gray-400 hover:text-primary transition-colors"
                  >Figuras</a
                >
              </li>
              <li>
                <a
                  href="#bustos"
                  class="text-gray-400 hover:text-primary transition-colors"
                  >Bustos</a
                >
              </li>
              <li>
                <a
                  href="#personalizados"
                  class="text-gray-400 hover:text-primary transition-colors"
                  >Personalizados</a
                >
              </li>
            </ul>
          </div>

          <!-- Contacto -->
          <div>
            <h3 class="text-lg font-semibold mb-4 border-b border-primary pb-2">
              Contacto
            </h3>
            <ul class="space-y-2">
              <li class="flex items-start">
                <span
                  class="w-5 h-5 flex items-center justify-center mt-1 mr-2 text-primary"
                >
                  <i class="ri-instagram-line"></i>
                </span>
                <span class="text-gray-400">@nombre_usuario</span>
              </li>
              <li class="flex items-start">
                <span
                  class="w-5 h-5 flex items-center justify-center mt-1 mr-2 text-primary"
                >
                  <i class="ri-mail-line"></i>
                </span>
                <span class="text-gray-400">info@ejemplo.com</span>
              </li>
              <li class="flex items-start">
                <span
                  class="w-5 h-5 flex items-center justify-center mt-1 mr-2 text-primary"
                >
                  <i class="ri-whatsapp-line"></i>
                </span>
                <span class="text-gray-400">+34 600 123 456</span>
              </li>
            </ul>
          </div>
        </div>

        <div
          class="border-t border-gray-800 mt-10 pt-6 text-center text-gray-500"
        >
          <p>
            &copy; 2025 Impresiones 3D Personalizadas. Todos los derechos
            reservados.
          </p>
        </div>
      </div>
    </footer>

    <script>
      // Menú móvil
      const mobileMenuButton = document.getElementById("mobile-menu-button");
      const mobileMenu = document.getElementById("mobile-menu");

      mobileMenuButton.addEventListener("click", () => {
        mobileMenu.classList.toggle("hidden");
      });

      // Cerrar menú al hacer clic en un enlace
      const mobileLinks = mobileMenu.querySelectorAll("a");
      mobileLinks.forEach((link) => {
        link.addEventListener("click", () => {
          mobileMenu.classList.add("hidden");
        });
      });

      // Filtros de galería (funcionalidad básica)
      const filterButtons = document.querySelectorAll(".container button");
      filterButtons.forEach((button) => {
        button.addEventListener("click", () => {
          filterButtons.forEach((btn) =>
            btn.classList.remove("active", "border-primary", "text-primary"),
          );
          button.classList.add("active", "border-primary", "text-primary");
        });
      });
    </script>
  </body>
</html>
