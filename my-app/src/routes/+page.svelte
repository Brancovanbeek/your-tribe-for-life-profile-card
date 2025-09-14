    <picture class="img">
      <!-- AVIF voor moderne browsers -->
      <source 
          srcset="
              /src/lib/assets/Branco-mugshot-400.avif 400w,
              /src/lib/assets/Branco-mugshot-500.avif 500w,
              /src/lib/assets/Branco-mugshot-700.avif 700w
          "
          sizes="33vw"
          type="image/avif"
      >
  
      <!-- WebP voor iets oudere browsers -->
      <source 
          srcset="
              /src/lib/assets/Branco-mugshot-400.webp 400w,
              /src/lib/assets/Branco-mugshot-500.webp 500w,
              /src/lib/assets/Branco-mugshot-700.webp 700w
          "
          sizes="33vw"
          type="image/webp"
      >
  
      <!-- PNG fallback -->
      <img 
          src="/src/lib/assets/Branco-mugshot-700.png"
          alt="Branco van Beek"
          width="320"
          height="auto"
          loading="lazy"
      />
    </picture>
