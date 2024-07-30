<script>
    import { onMount } from 'svelte';
  
    const appName = import.meta.env.VITE_APP_NAME;
  
    onMount(() => {
      document.title = `${appName}`;
    });

    const pageTitle = "Proto Angelo's First Portfolio";
    const pageDescription = "Take your time exploring what he has created for you. Enjoy the tour!";
    const ogImage = "https://webprofile-theta.vercel.app/assets/images/metapreview.webp";
    const url = "https://webprofile-theta.vercel.app/";
  </script>

<svelte:head>
    <!-- Primary Meta Tags -->
    <title>{pageTitle}</title>
    <meta name="description" content={pageDescription}>
  
    <!-- Open Graph / Facebook -->
    <meta property="og:type" content="website">
    <meta property="og:url" content={url}>
    <meta property="og:title" content={pageTitle}>
    <meta property="og:description" content={pageDescription}>
    <meta property="og:image" content={ogImage}>
  
    <!-- Twitter -->
    <meta property="twitter:card" content="summary_large_image">
    <meta property="twitter:url" content={url}>
    <meta property="twitter:title" content={pageTitle}>
    <meta property="twitter:description" content={pageDescription}>
    <meta property="twitter:image" content={ogImage}>
    <meta name="robots" content="index, follow">
  
    <!-- Cross Browser icon -->
    <!-- <link rel="shortcut icon" href="/assets/images/VAV.ico">
    <link rel="icon" type="image/vnd.microsoft.icon" href="/assets/images/VAV.ico">
    <link rel="icon" type="image/x-icon" href="/assets/images/VAV.ico">
    <link rel="icon" href="/assets/images/VAV.ico"> -->
  </svelte:head>
  <!-- Your component or layout content -->
  <slot />
  