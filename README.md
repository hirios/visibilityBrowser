# visibilityBrowser



https://github.com/wpears/dont/blob/master/dont.js


https://stackoverflow.com/questions/58772369/headless-google-chrome-how-to-prevent-sites-to-know-whether-their-window-is-foc


https://stackoverflow.com/questions/69268755/disable-page-visibility-api-in-chrome-extension-for-facebook


https://stackoverflow.com/questions/47660653/chrome-extension-how-to-disable-page-visibility-api


for (event_name of ["visibilitychange", "webkitvisibilitychange", "blur"]) {
  window.addEventListener(event_name, function(event) {
        event.stopImmediatePropagation();
    }, true);
}



document.querySelector('[id="teste"]').addEventListener('click', function(event) {
  console.log('primeiroEvento');
})


document.querySelector('[id="teste"]').addEventListener('click', function(el) {
  console.log('segundoEvento');
  el.stopImmediatePropagation();
}, true)
