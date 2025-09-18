<script>
    const { member } = $props();
</script>

<picture class="mugshot-img">
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
        alt="{member.name}"
        width="31.25rem" 
        height="auto"
        loading="lazy"
    /> <!-- 500px → 31.25rem -->
</picture>

<style>
    .mugshot-img {
        position: relative;
        display: flex;
        justify-content: center;
        width: 100%;
    }
    img {
        width: 100%;
        height: auto;
        max-width: 18.75rem; /* 300px → 18.75rem */
        margin-top: -3rem;
    }
</style>
