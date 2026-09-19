# Traduki uzantointerfacajn elementojn en Esperanton per AI

Estas prezentata Tampermonkey-skripto, por traduki uzantointerfacajn elementojn en Esperanton per la OpenAI-API. La skripto funkcias en Google Docs kaj aliaj retejoj.

## Instalado

1. Instalu **Tampermonkey** por via krozilo lau la instruoj che [tampermonkey.net](https://www.tampermonkey.net/).
2. Uzu au kreu [OpenAI-API-shlosilon](https://platform.openai.com/api-keys).
3. Malfermu [traduki.js](./traduki.js), alklaku **Raw** kaj kopiu la tutan kodon.
4. En la menuo de Tampermonkey elektu **krei novan skripton**. Forigu la ekzemplan kodon kaj algluu la kopiitan kodon.
5. Enmetu vian OpenAI-API-shlosilon en la linion kun `const OPENAI_API_KEY = 'sk-...';`.

6. Konservu la skripton per **Ctrl+S** au **Cmd+S** kaj certigu, ke ghi estas aktivigita.

## Uzado

1. Malfermu au aktualigu la deziratan retpaghon.
2. Alklaku **“Traduki menuojn → EO”** malsupre dekstre.
3. Malfermu menuojn kaj submenuojn, kiel kutime. Novaj tekstoj estas automate tradukataj; tio povas dauri kelkajn sekundojn.
4. Alklaku la butonon denove por fari pauzon. Por restarigi la originalajn tekstojn, aktualigu la retpaghon.

Se la butono mankas, kontrolu la permesojn de Tampermonkey kaj eventualajn instruojn pri aktivigo de uzantoskriptoj.

## Atentu

- Menuaj tekstoj estas sendataj al OpenAI kaj povas enteni dosiernomojn au aliajn personajn informojn.
- API-uzado povas kauzi kostojn.
- **Neniam publikigu vian API-shlosilon**.
- Ne chiuj retejoj kaj menuotipoj estas subtenataj.

Por limigi la skripton al Google Docs, anstatauigu la ekzistantan `@match`-linion per `// @match        https://docs.google.com/*`.
