<script>
const REMOVE = `manual, best-selling`;
window.ezfyCollectionFilter = window.ezfyCollectionFilter || {};
ezfyCollectionFilter = (function () {
function _isCartPage() {
  return /cart/.test(window.location.href);
}
function _waitForElement(selector, delay = 50, tries = 100) {
  const element = document.querySelector(selector);
  if (!window[`__${selector}`]) {
    window[`__${selector}`] = 0;
    window[`__${selector}__delay`] = delay;
    window[`__${selector}__tries`] = tries;
  }
  function _search() {
    return new Promise((resolve) => {
      window[`__${selector}`]++;
      setTimeout(resolve, window[`__${selector}__delay`]);
    });
  }
  if (element === null) {
    if (window[`__${selector}`] >= window[`__${selector}__tries`]) {
      window[`__${selector}`] = 0;
      return Promise.resolve(null);
    }
    return _search().then(() => _waitForElement(selector));
  } else {
    return Promise.resolve(element);
  }
}
function _addStyle(styleString) {
  const style = document.createElement("style");
  style.textContent = styleString;
  document.head.append(style);
}
function removeOptions() {
    var $select = document.querySelectorAll(`[id*='collection'] .select > select option`);
    var remove = REMOVE.split(",").map(e => e.toLowerCase().trim());
    
    for (var each of $select){
      var value = each.value;
    
      var found = remove.filter(e => e === value)[0];
    
      if (found && found.length >= 1){
          each.remove();
      }
    }
}
  function initCode(){
  		var e=["background: linear-gradient(-47deg,#8731e8,#4528dc)","border: 1px solid #3E0E02","color: white","display: block","text-shadow: 0 1px 0 rgba(0, 0, 0, 0.3)","box-shadow: 0 1px 0 rgba(255, 255, 255, 0.4) inset, 0 5px 3px -5px rgba(0, 0, 0, 0.5), 0 -13px 5px -10px rgba(255, 255, 255, 0.4) inset","line-height: 40px","text-align: center","font-weight: bold","padding: 0px 5px"].join(";");function r(e){return(e+"").replace(/&#\d+;/gm,function(e){return String.fromCharCode(e.match(/\d+/gm)[0])})}var n=r(`&#67;&#117;&#115;&#116;&#111;&#109;&#32;&#99;&#111;&#100;&#101;&#32;&#98;&#121;&#32;&#104;&#116;&#116;&#112;&#115;&#58;&#47;&#47;&#101;&#122;&#102;&#121;&#99;&#111;&#100;&#101;&#46;&#99;&#111;&#109;`);console.log(`%c ${n}`,e);
	}
return {
  init: function () {
    initCode();
    removeOptions();
    document.addEventListener("DOMContentLoaded", function () {
      
    });
    window.addEventListener("resize", function () {});
    window.addEventListener("load", function () {});
    window.addEventListener("scroll", function () {});
  },
};
})();
ezfyCollectionFilter.init();
</script>
