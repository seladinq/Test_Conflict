const toggleButton = document.getElementById('theme-toggle');
const body = document.body;

toggleButton.addEventListener('click', () => {
    body.classList.toggle('dark-mode');

    // Ndrysho ikonën
    if(body.classList.contains('dark-mode')){
        toggleButton.textContent = '☀️'; // Dielli kur është dark mode
    } else {
        toggleButton.textContent = '🌙'; // Hëna kur është light mode
    }
});
