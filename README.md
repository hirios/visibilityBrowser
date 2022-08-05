# visibilityBrowser



https://github.com/wpears/dont/blob/master/dont.js


https://stackoverflow.com/questions/58772369/headless-google-chrome-how-to-prevent-sites-to-know-whether-their-window-is-foc


https://stackoverflow.com/questions/69268755/disable-page-visibility-api-in-chrome-extension-for-facebook


https://stackoverflow.com/questions/9515704/use-a-content-script-to-access-the-page-context-variables-and-functions/9517879#9517879



document.querySelector('[id="teste"]').addEventListener('click', function(event) {
  console.log('primeiroEvento');
})


document.querySelector('[id="teste"]').addEventListener('click', function(el) {
  console.log('segundoEvento');
  el.stopImmediatePropagation();
}, true)
