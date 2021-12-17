<template>
  <section
    id="contact"
    class="contact flex flex-col h-screen my-auto items-center bgimg bg-cover"
  >
    <div class="container">
      <div class="mb-4">
        <h2 class="font-bold text-4xl text-gray-800">Contact Us</h2>
      </div>
      <div class="md:flex">
        <div class="w-full mb-8 md:w-1/3">
          <div class="">
            <h3 class="font-open-sans font-semibold text-2xl text-gray-800">
              PT-Teknik
            </h3>
            <p class="text-gray-700 font-open-sans">
              Cras fermentum odio eu feugiat. Justo eget magna fermentum iaculis
              eu non diam phasellus. Scelerisque felis imperdiet proin fermentum
              leo. Amet volutpat consequat mauris nunc congue.
            </p>
            <div class="social-links">
              <a href="#" class="twitter"><i class="icofont-twitter"></i></a>
              <a href="#" class="facebook"><i class="icofont-facebook"></i></a>
              <a href="#" class="instagram"
                ><i class="icofont-instagram"></i
              ></a>
              <a href="#" class="linkedin"><i class="icofont-linkedin"></i></a>
            </div>
          </div>
        </div>

        <div class="w-full md:w-1/3" data-aos="fade-up" data-aos-delay="200">
          <div class="info">
            <div class="flex items-start mb-8">
              <i class="fas ml-1 text-3xl fa-map-marker-alt text-green-400"></i>
              <p class="pl-4 text-gray-700">
                Personalhuset <br />Oxelösund, Aspaleden 613 31
              </p>
            </div>

            <div class="flex items-start my-8">
              <i class="fas fa-envelope-open text-3xl text-green-400"></i>
              <p class="pl-3 text-gray-700">info@example.com</p>
            </div>

            <div class="flex items-start my-8">
              <i class="fas fa-id-card-alt text-3xl text-green-400"></i>
              <p class="pl-3 text-gray-700">+0155-25-40-00s</p>
            </div>
          </div>
        </div>

        <div class="w-full md:w-1/3" data-aos="fade-up" data-aos-delay="300">
          <form
            action="forms/contact.php"
            method="post"
            role="form"
            class="php-email-form"
          >
            <div class="form-group">
              <input
                type="text"
                name="name"
                class="w-full border mb-2 px-3 py-2"
                id="name"
                placeholder="Your Name"
                data-rule="minlen:4"
                data-msg="Please enter at least 4 chars"
              />
              <div class="validate"></div>
            </div>
            <div class="form-group">
              <input
                type="email"
                class="w-full border mb-2 px-3 py-2"
                name="email"
                id="email"
                placeholder="Your Email"
                data-rule="email"
                data-msg="Please enter a valid email"
              />
              <div class="validate"></div>
            </div>

            <div class="form-group">
              <textarea
                class="w-full border mb-2 px-3 py-2"
                name="message"
                rows="5"
                data-rule="required"
                data-msg="Please write something for us"
                placeholder="Message"
              ></textarea>
              <div class="validate"></div>
            </div>

            <div class="text-center">
              <button
                type="submit"
                class="bg-blue-600 text-gray-200 rounded px-4 py-2 font-open-sans"
              >
                Send Message
              </button>
            </div>
          </form>
        </div>
      </div>
    </div>
  </section>
</template>
