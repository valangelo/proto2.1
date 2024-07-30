<script>
    import { page } from '$app/stores';
    import { VITE_APP_NAME, VITE_APP_DESCRIPTION, VITE_APP_URL, VITE_APP_IMAGE } from '$env/static/private';
  
    const pageTitle = VITE_APP_NAME;
    const pageDescription = VITE_APP_DESCRIPTION;
    const pageUrl = VITE_APP_URL;
    const ogImage = VITE_APP_IMAGE;
  </script>
  
  <svelte:head>
    <!-- Primary Meta Tags -->
    <title>{pageTitle}</title>
    <meta name="description" content={pageDescription} />
  
    <!-- Open Graph / Facebook -->
    <meta property="og:type" content="website" />
    <meta property="og:url" content={pageUrl} />
    <meta property="og:title" content={pageTitle} />
    <meta property="og:description" content={pageDescription} />
    <meta property="og:image" content={ogImage} />
  
    <!-- Twitter -->
    <meta property="twitter:card" content="summary_large_image" />
    <meta property="twitter:url" content={pageUrl} />
    <meta property="twitter:title" content={pageTitle} />
    <meta property="twitter:description" content={pageDescription} />
    <meta property="twitter:image" content={ogImage} />
  
    <!-- Robots -->
    <meta name="robots" content="index, follow" />
  
    <!-- Cross Browser icon -->
    <link rel="shortcut icon" href="/assets/images/VAV.ico" />
    <link rel="icon" type="image/vnd.microsoft.icon" href="/assets/images/VAV.ico" />
    <link rel="icon" type="image/x-icon" href="/assets/images/VAV.ico" />
  </svelte:head>
  