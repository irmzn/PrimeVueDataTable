# Unstyled Mode

Step 1 - https://primevue.org/vite/

npm install primevue

Step 2 - https://primevue.org/theming/unstyled/
app.use(PrimeVue, {
    unstyled: true
});

--------------------------------------------------------------

# Styled Mode

Step 1 - https://primevue.org/vite/

npm install @primevue/themes

Step 2 - https://primevue.org/theming/styled/

import PrimeVue from 'primevue/config';

import Aura from '@primevue/themes/aura';
app.use(PrimeVue, {
    theme: {
        preset: Aura
    }
});

# Other Test

import Noir from './presets/Noir.js';
app.use(PrimeVue, {
    theme: {
        preset: Noir,
        options: {
            prefix: 'p',
            darkModeSelector: '.p-dark',
            cssLayer: false,
        }
    }
});

app.use(PrimeVue);
