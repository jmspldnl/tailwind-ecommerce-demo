<template>
  <div class="flex flex-col my-4">
    <div class="flex">
      <div class="box-border p-4 w-1/2">
        <div class="bg-gray-100 relative" style="padding-bottom:100%">
          <img class="absolute inset-0 h-full w-full object-cover" />
        </div>
      </div>
      <div class="box-border p-4 w-1/2">
        <h2 class="text-2xl">Product Name</h2>
        <div class="my-4">
          <p>
            <span class="text-xl">$29.99</span>
            <s>$49.99</s><br />
            <span class="text-red-500">
              You save $20.00 ({{ Math.floor((20 / 49.99) * 100) }}%)
            </span>
          </p>
        </div>
        <button
          class="bg-blue-500 text-white my-4 px-8 py-4 uppercase hover:bg-blue-400 transition-colors"
        >
          Add To Cart
        </button>
        <ul class="list-disc m-4">
          <li>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</li>
          <li>
            Curabitur scelerisque, diam eget pellentesque vulputate, massa ex
            molestie nunc, vitae vehicula justo est vel magna.
          </li>
          <li>Quisque aliquet eros et bibendum lacinia.</li>
          <li>Proin malesuada diam at accumsan lacinia.</li>
          <li>
            Nunc congue turpis et orci eleifend, at bibendum est ullamcorper.
          </li>
          <li>Vivamus sed finibus diam.</li>
          <li>Suspendisse potenti.</li>
          <li>Morbi a erat tellus.</li>
          <li>In hac habitasse platea dictumst.</li>
          <li>Aliquam convallis tortor et risus dictum hendrerit.</li>
          <li>Ut vitae ante tristique, posuere ex ac, feugiat purus.</li>
          <li>Etiam in pellentesque sapien, ac euismod tortor.</li>
          <li>Pellentesque sit amet euismod velit.</li>
          <li>Nam libero tortor, cursus vel leo in, commodo mollis sem.</li>
          <li>Phasellus ac viverra mi.</li>
        </ul>
      </div>
    </div>
    <div class="m-4">
      <ul class="flex border-b">
        <li class="-mb-px mr-1">
          <a
            class="bg-white inline-block border-l border-t border-r rounded-t py-2 px-4 text-blue-700 font-semibold"
            href="#"
            >Active</a
          >
        </li>
        <li class="mr-1">
          <a
            class="bg-white inline-block py-2 px-4 text-blue-500 hover:text-blue-800 font-semibold"
            href="#"
            >Tab</a
          >
        </li>
        <li class="mr-1">
          <a
            class="bg-white inline-block py-2 px-4 text-blue-500 hover:text-blue-800 font-semibold"
            href="#"
            >Tab</a
          >
        </li>
        <li class="mr-1">
          <a
            class="bg-white inline-block py-2 px-4 text-gray-400 font-semibold"
            href="#"
            >Tab</a
          >
        </li>
      </ul>
      <div>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur
          scelerisque, diam eget pellentesque vulputate, massa ex molestie nunc,
          vitae vehicula justo est vel magna. Quisque aliquet eros et bibendum
          lacinia. Proin malesuada diam at accumsan lacinia. Nunc congue turpis
          et orci eleifend, at bibendum est ullamcorper. Vivamus sed finibus
          diam. Suspendisse potenti. Morbi a erat tellus. In hac habitasse
          platea dictumst. Aliquam convallis tortor et risus dictum hendrerit.
          Ut vitae ante tristique, posuere ex ac, feugiat purus. Etiam in
          pellentesque sapien, ac euismod tortor. Pellentesque sit amet euismod
          velit. Nam libero tortor, cursus vel leo in, commodo mollis sem.
          Phasellus ac viverra mi.
        </p>
        <p>
          Donec vestibulum maximus orci, quis vulputate est gravida eu.
          Suspendisse dictum sem vel dui suscipit, id eleifend lorem tincidunt.
          Class aptent taciti sociosqu ad litora torquent per conubia nostra,
          per inceptos himenaeos. Donec ultrices tristique arcu, ut tempor orci
          dictum sit amet. Etiam sed volutpat arcu, eu sagittis augue. Mauris
          tempus sagittis velit ac suscipit. Morbi id quam commodo, maximus
          risus at, ornare ex. Interdum et malesuada fames ac ante ipsum primis
          in faucibus.
        </p>
        <p>
          Etiam nisl ante, interdum id vulputate cursus, viverra nec quam.
          Quisque neque felis, commodo at massa nec, condimentum lacinia tellus.
          Suspendisse scelerisque dapibus commodo. Suspendisse sem nisi,
          tincidunt semper justo vitae, interdum pretium augue. Vivamus non
          tellus quam. Fusce vitae hendrerit est. Donec ac egestas nunc. Ut
          ullamcorper quam sagittis, eleifend metus at, tempor metus. Nam
          faucibus facilisis urna sit amet molestie. Nam ac ultrices eros. Nam
          venenatis convallis ipsum, non rutrum tortor finibus ac. Integer
          euismod ornare tellus placerat facilisis. Aenean nisl orci, suscipit
          vel pretium fermentum, hendrerit eu enim. Donec pulvinar turpis
          pretium augue facilisis sollicitudin. Phasellus bibendum eros ut dui
          luctus iaculis.
        </p>
        <p>
          Pellentesque ultrices turpis id vehicula imperdiet. Vestibulum sodales
          ex a rutrum lobortis. Etiam eget tempor ex. Ut luctus pulvinar urna at
          pellentesque. Etiam at mauris nec neque elementum posuere ut ut dolor.
          Sed vestibulum, sapien vitae lobortis fermentum, enim libero venenatis
          dui, nec sollicitudin nulla lorem eu lorem. Nullam nec turpis bibendum
          ex semper commodo a non diam. Phasellus faucibus condimentum leo, non
          pulvinar nunc tempus id. Proin aliquam tincidunt ante sit amet
          eleifend. Sed a neque tortor. Aliquam quis urna imperdiet, volutpat
          velit id, volutpat lorem. Nullam quis tempor velit. Cras sagittis
          molestie laoreet. Donec dictum sodales neque, nec molestie mi gravida
          nec.
        </p>
        <p>
          Cras maximus purus aliquam sem fringilla facilisis. Maecenas convallis
          luctus tellus a euismod. Orci varius natoque penatibus et magnis dis
          parturient montes, nascetur ridiculus mus. Nullam imperdiet tortor
          vitae fermentum elementum. Pellentesque iaculis ultrices dolor nec
          dictum. In dolor mauris, vestibulum a ullamcorper quis, tristique sed
          nisi. Suspendisse consequat lacinia dolor vel volutpat.
        </p>
      </div>
    </div>
  </div>
</template>
