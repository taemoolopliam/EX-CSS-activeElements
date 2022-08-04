# EX-CSS-activeElements
Examples of active colors in javascript and jquery.


# jquery

    $(".tab-item").click(function (event) {
      $(".tab-item").removeClass("tab-item-active");
      event.target.classList.add("tab-item-active");
    });

# javascript

      const tabItem = document.getElementsByClassName("tab-item");
      for (var i = 0, length = tabItem.length; i < length; i++) {
        tabItem[i].onclick = function (event) {
          var findActive = document.querySelector("div.tab-item-active");
          if (findActive) findActive.classList.remove("tab-item-active");
          event.target.classList.add("tab-item-active");
        };
      }
