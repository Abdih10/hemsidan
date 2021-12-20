<template>
  <div class="w-full md:w-96 md:max-w-full mx-auto">
    <div class="p-6 border border-gray-300 sm:rounded-md">
      <form method="POST">
        <label class="block mb-6">
          <span class="text-gray-700">Namn</span>
          <input
            type="text"
            name="name"
            class="block w-full mt-1 border-gray-300 rounded-md shadow-sm focus:border-indigo-300 focus:ring focus:ring-indigo-200 focus:ring-opacity-50"
            placeholder="Abdi Hussein"
          />
        </label>
        <label class="block mb-6">
          <span class="text-gray-700">Email address</span>
          <input
            name="email"
            type="email"
            class="block w-full mt-1 border-gray-300 rounded-md shadow-sm focus:border-indigo-300 focus:ring focus:ring-indigo-200 focus:ring-opacity-50"
            placeholder="info@ssab.com"
            required
          />
        </label>
        <label class="block mb-6">
          <span class="text-gray-700">Anställningsnummer</span>
          <input
            type="text"
            name="name"
            class="block w-full mt-1 border-gray-300 rounded-md shadow-sm focus:border-indigo-300 focus:ring focus:ring-indigo-200 focus:ring-opacity-50"
            placeholder="0000"
          />
        </label>
        <label for="name" class="text-base leading-7 text-blueGray-500"
          >Datum</label
        >
        <input
          type="date"
          id="date"
          name="date"
          placeholder="name"
          class="w-full px-4 py-2 mt-2 mr-4 text-base text-black transition duration-500 ease-in-out transform rounded-lg bg-gray-100 focus:border-blueGray-500 focus:bg-white focus:outline-none focus:shadow-outline focus:ring-2 ring-offset-current ring-offset-2"
        />
        <label class="block mb-6">
          <span class="text-gray-700">Tid</span>
          <input
            type="text"
            name="Tid"
            class="block w-full mt-1 border-gray-300 rounded-md shadow-sm focus:border-indigo-300 focus:ring focus:ring-indigo-200 focus:ring-opacity-50"
            placeholder="08:00"
          />
        </label>
        <label for="name" class="text-base leading-7 text-blueGray-500"
          >Supporttype</label
        >
        <select
          class="w-full px-4 py-2 mt-2 text-base text-black transition duration-500 ease-in-out transform rounded-lg bg-gray-100 focus:border-blueGray-500 focus:bg-white focus:outline-none focus:shadow-outline focus:ring-2 ring-offset-current ring-offset-2"
        >
          <option>Felavhjälpning under dagtid</option>
          <option>Felavhjälpning under icke dagtid</option>
          <option>Förbättring</option>
          <option>Updatering</option>
        </select>
        <label class="block mb-6">
          <span class="text-gray-700">System</span>
          <input
            type="text"
            name="name"
            class="block w-full mt-1 border-gray-300 rounded-md shadow-sm focus:border-indigo-300 focus:ring focus:ring-indigo-200 focus:ring-opacity-50"
            placeholder="ex: BSL732"
          />
        </label>
        <label for="name" class="text-base leading-7 text-blueGray-500"
          >Systemtype</label
        >
        <select
          class="w-full px-4 py-2 mt-2 text-base text-black transition duration-500 ease-in-out transform rounded-lg bg-gray-100 focus:border-blueGray-500 focus:bg-white focus:outline-none focus:shadow-outline focus:ring-2 ring-offset-current ring-offset-2"
        >
          <option>Processystem (proview)</option>
          <option>Operatörssyem (proview)</option>
          <option>Nivå 2-system</option>
          <option>PSS-hårdvara</option>
          <option>Övrigt</option>
        </select>
        <label for="name" class="text-base leading-7 text-blueGray-500"
          >Felkategori</label
        >
        <select
          class="w-full px-4 py-2 mt-2 text-base text-black transition duration-500 ease-in-out transform rounded-lg bg-gray-100 focus:border-blueGray-500 focus:bg-white focus:outline-none focus:shadow-outline focus:ring-2 ring-offset-current ring-offset-2"
        >
          <option>PSS-hårdvara</option>
          <option>Givare, ställdon mm.</option>
          <option>Fältbussar inkl. IO</option>
          <option>Program (mjukvara)</option>
          <option>Nätverk/nivå 3</option>
          <option>Handhavande operatör/underhåll</option>
          <option>Handhavande kontruktör</option>
          <option>Övrigt</option>
        </select>
        <label class="block mb-6">
          <span class="text-gray-700">Problembeskrivning</span>
          <textarea
            name="message"
            class="block w-full mt-1 border-gray-300 rounded-md shadow-sm focus:border-indigo-300 focus:ring focus:ring-indigo-200 focus:ring-opacity-50"
            rows="3"
            placeholder="Fri text"
          ></textarea>
        </label>
        <label class="block mb-6">
          <span class="text-gray-700">Åtgärd</span>
          <textarea
            name="message"
            class="block w-full mt-1 border-gray-300 rounded-md shadow-sm focus:border-indigo-300 focus:ring focus:ring-indigo-200 focus:ring-opacity-50"
            rows="3"
            placeholder="Fri text"
          ></textarea>
        </label>
        <label class="block mb-6">
          <span class="text-gray-700">Tidsgång</span>
          <input
            type="text"
            name="Tid"
            class="block w-full mt-1 border-gray-300 rounded-md shadow-sm focus:border-indigo-300 focus:ring focus:ring-indigo-200 focus:ring-opacity-50"
            placeholder="08:00"
          />
        </label>
        <label for="name" class="text-base leading-7 text-blueGray-500"
          >Felkategori</label
        >
        <select
          class="w-full px-4 py-2 mt-2 text-base text-black transition duration-500 ease-in-out transform rounded-lg bg-gray-100 focus:border-blueGray-500 focus:bg-white focus:outline-none focus:shadow-outline focus:ring-2 ring-offset-current ring-offset-2"
        >
          <option>Problem löst permanent</option>
          <option>Problem löst temporärt</option>
          <option>Olöst</option>
        </select>
        <div class="mb-6">
          <button
            type="submit"
            class="h-10 px-5 text-indigo-100 bg-indigo-700 rounded-lg transition-colors duration-150 focus:shadow-outline hover:bg-indigo-800"
          >
            Contact Us
          </button>
        </div>
        <div>
          <div class="mt-2 text-gray-700 text-right text-xs">
            by
            <a
              href="https://herotofu.com"
              class="hover:underline"
              target="_blank"
              >PT-Teknik</a
            >
          </div>
        </div>
      </form>
    </div>
  </div>
</template>
