<template>
  <section class="relative bg-repeat-x py-8" style="background-image: url('/pattern.svg');">
    <div class="sm:px-12 lg:mx-auto lg:max-w-screen-xl">
      <p class="text-lg font-medium text-zinc-100">
        Chcę się zaaangażować...
      </p>
      <h2 class="relative mb-5 text-4xl font-extrabold text-zinc-100 underline decoration-red-400/25 decoration-[1rem] underline-offset-[-0.5rem]" style="text-decoration-skip-ink: none;">
        Dołącz do nas!
      </h2>
      <p class="mb-5 leading-normal text-zinc-100">
        Jeżeli uczysz się programować, to bierz udział w naszych spotkaniach aby dalej poszerzać swoją wiedzę. A jeżeli jesteś już w tym naprawdę dobry, to twórz z nami nowe projekty.
      </p>
      <div class="grid grid-flow-row gap-4 lg:grid-flow-col lg:grid-cols-2 auto-rows-fr">
        <card title="Znajdź nas!">
          <template #description>
            Jesteśmy dostępni na <a href="#" class="text-[#5865F2] underline">Discordzie</a> oraz <a href="#" class="text-[#17A9FD] underline">Facebooku</a>, a dla osób z zewnątrz pod adresem mailowym. Nasze “biuro” znajduje się w budynku 34 SGGW w sali 3/77.
          </template>
        </card>
        <card title="Współpraca" description="Chętnie nawiążemy współpracę z firmami zewnętrznymi oraz innymi organizacjami studenckimi. Zapraszamy do wspólnej organizacji spotkań/warsztatów dla studentów informatyki SGGW oraz wszelkich rozmów w sprawie nowych projektów i aplikacji." />
      </div>
    </div>
  </section>
</template>
