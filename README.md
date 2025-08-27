<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Styled Search Button</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <button class="search-button">
        <span class="search-prompt">
            <span class="search-icon">🔍</span>
            <span>Search...</span>
        </span>

        <span class="search-shortcut">Ctrl+K</span>
    </button>

</body>
</html>

/*css*/
/* Stilizimi bazik i faqes për shembull */
body {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    background-color: #f0f2f5;
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
}

/* --- KY ËSHTË KODI KRYESOR PËR BUTONIN --- */

.search-button {
    /* Hapi 1: E kthejmë butonin në një kontejner Flexbox. Kjo është pjesa kyçe! */
    display: flex;
    
    /* Hapi 2: I shtyjmë dy elementët fëmijë (span-et) në skajet e kundërta */
    justify-content: space-between;

    /* Hapi 3: I rreshtojmë vertikalisht në qendër */
    align-items: center;

    /* Pjesa tjetër është stilim për pamjen */
    width: 240px;
    padding: 8px 12px;
    border: 1px solid #d1d5db; /* Ngjyrë gri e lehtë */
    border-radius: 8px;
    background-color: #f9fafb;
    color: #6b7280; /* Ngjyrë gri për tekstin */
    font-size: 14px;
    cursor: pointer;
    transition: border-color 0.2s;
}

.search-button:hover {
    border-color: #9ca3af; /* Theksohet pak kur kalon mausi sipër */
}

/* Stilizimi për pjesën e majtë (ikonën dhe tekstin) */
.search-prompt {
    display: flex;
    align-items: center;
}

.search-icon {
    margin-right: 8px; /* Krijon hapësirë mes lupës dhe tekstit "Search..." */
}

/* Stilizimi për shkurtoren (Ctrl+K) */
.search-shortcut {
    background-color: #f3f4f6;
    border: 1px solid #d1d5db;
    padding: 2px 6px;
    border-radius: 4px;
    font-size: 12px;
    color: #374151;
}
