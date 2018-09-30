---
layout: post
title: Please Do Not Erase
---

<head>
  <script src="/js/jquery-1.11.2.min.js"></script>
  <script>
  let words = {
    "IMG_2141": [ "the force", "weeping angel", "replication experiments", "analysis", "auditory", "signal", "processing", "ML" ],
    "IMG_2142": [ "sin", "cos", "cxt", "lambda", "xo", "t2" ],
    "IMG_2143": [ "shack", "cord", "printer filament", "study", "engines", "motor oil", "curvature", "rocket", "parachute" ],
    "IMG_2145": [ "small", "waterproof", "throttle", "dashboard", "organized", "servicable", "IP65", "BJ45", "AMPSEAL" ],
    "IMG_2146": [ "motor", "sprocket", "belt", "water" ],
    "IMG_2147": [ "lab", "status", "FPGA", "circuits", "vivado", "checkout" ],
    "IMG_2148": [ "debrief", "insulators", "semiconductors", "metals", "conceptuals", "capacitance", "monday", "chassis" ],
    "IMG_2149": [ "chassis", "mounting", "arduino", "reliably", "ASCII", "serial", "P-up", "tune", "constant", "IR1", "IR2" ],
    "IMG_2150": [ "1101", "Iy", "IR1", "IR2", "sensor", "on line" ],
    "IMG_2151": [ "da", "mathematica", "potential will grow", "with respect", "along a line" ],
    "IMG_2154": [ "sss", "dxdydz", "not symmetric", "enough", "superposition" ],
    "IMG_2156": [ "find potential", "cookie", "dv", "jwl", "E" ],
    "IMG_2158": [ "case 1", "pastry", "end of line", "loop", "CAD", "drill", "connector", "abs" ],
    "IMG_2159": [ "dennett", "key", "yorick", "hubert", "hamlet", "comp", "brain", "who", "normal", "start here" ],
    "IMG_2160": [ "where", "youuuuu", "I'm so sorry", "yorick", "hamlet" ],
    "IMG_2162": [ "DC", "3-Phase", "AC", "generator", "load", "brushless", "less safe", "not scalable", "6 lines" ],
    "IMG_2164": [ "I doubt", "david", "exists", "see hear feel think" ],
    "IMG_2166": [ "clark", "john's head", "martian", "multiple mindless", "independent", "processes", "language", "implications", "predates", "forgets", "unified", "correspond", "intimicy", "inner echo", "alien source" ],
    "IMG_2167": [ "reliability", "warehouses", "cheaper", "DC", "long term savings", "long distances" ],
    "IMG_2168": [ "limit", "admin", "json", "calculate", "ppb", "map", "graph", "routes", "insert", "device", "scan" ],
    "IMG_2169": [ "R(3,3)", "red/blue", "5 edges", "K3", "edges", "however", "colored", "php" ],
    "IMG_2170": [ "1 Insulin", "2 FVIII", "3 Progesterene", "4 Aceso", "5 Epinephrine" ],
    "IMG_2171": [ "today", "11:10", "memes", "word bank", "o' connor", "capture the day" ],
    "IMG_2172": [ "drunk", "1/2", "2/3", "sober", "9/13", "Pr" ],
    "IMG_2173": [ "cancer", "sick", "sensitivity", "3%", "well", "0.5", "FOBT", ],
    "IMG_2175": [ "length", "is not", "changing", "l1", "a1" ],
    "IMG_2177": [ "self-actualization", "acceptance", "social", "living", "food", "water", "shelter" ],
    "IMG_2178": [ "we need", "social imagination", "envision", "just", "alternatives" ],
    "IMG_2179": [ "elements of", "value", "cool tech", "lowell", "outrospections", "TSA", "sri lanka" ],
    "IMG_2180": [ "semantic", "database", "early", "team", "subteam", "ECE", "fred", "modeling", "naming", "documentation" ],
    "IMG_2182": [ "n", "2", "3", "4", "11", "011", "211", "112", "2110", "0110" ],
    "IMG_2183": [ "meta", "AC", "looking", "processing", "gathering new data", "classes", "by choice" ],
    "IMG_2184": [ "help", "me", "soldworkds", "design" ],
    "IMG_2186": [ "fear not", "citizens", "we shall", "feed upon", "cyber", "for all", "eternity", "gruel" ],
    "IMG_2187": [ "make", "models", "simple", "possible", "simpler", "but", "einstein", "matthew" ],
    "IMG_2188": [ "click", "beetle", "resting", "position", "triggered by", "take off", "poised", "peg" ],
    "IMG_2190": [ "teaming", "success", "hi", "five", "hand" ],
    "IMG_2191": [ "enable review", "graphics", "regedit", "search", "current user", "nv40", "dword", "workgarounds", "30008", "pray", "cool" ],
    "IMG_2192": [ "phoenix", "flies", "anytime", "never", "enough time" ],
    "IMG_2196": [ "let", "ninja", "know", "need", "extra", "components", "fishing wine", "etc" ],
    "IMG_2198": [ "for", "the", "laser", "cutter", "people" ],
    "IMG_2199": [ "why", "jump", "preadator", "bye!!", "???", "time to" ],
    "IMG_2200": [ "please", "replace", "anna", "&", "tim", "suction cup", "springs", "wire", "tubing", "rubber", "julia" ],
    "IMG_2201": [ "chain mail", "steel", "leggings", "ready", "machine", "shop", "crocs", "adventure", "straps", "slippers", "tuck", "roll up" ],
    "IMG_2202": [ "class", "motionmodel", "predict", "move", "map", "calc", "diff", "reading", "particle", "generate", "guess", "viz" ],
    "IMG_2203": [ "OCU", "motor", "world", "sense", "process", "rudder", "change objectives", "thing to do", "arbitrate", "prioritize" ]
  };

    function shuffle(a) {
      for (let i = a.length - 1; i > 0; i--) {
          const j = Math.floor(Math.random() * (i + 1));
          [a[i], a[j]] = [a[j], a[i]];
      }
      return a;
    }

    function googleLink(terms) {
      var link = "https://www.google.com/search?query="
      for (var term in terms) {
        link = link + term + "+"
      }
      return base
    }

    $(document).ready(function() {
      let image_names = shuffle(Object.keys(words)).slice(-3);
      console.log(image_names);
      for (var index in image_names) {
        let image_name = image_names[index]
        let terms = shuffle(words[image_name]).slice(-3);
        let href = googleLink(terms);
        $("div.images").append("<img src=\"/assets/img/project1/" + image_name + ".JPG\" href=\"" + href + "\" \/></br>");
      }
    });

    $("h1").text("Jquery works");
    $("p").text("swap");
  </script>
</head>

<div>
  <h1>Test 3</h1>
  <p>another test</p>
  <div class="images"></div>
  {% for image in site.static_files %}
    {% if image.path contains 'Ximg/project1' %}
      <img src="{{ site.baseurl }}{{ image.path }}" alt="image" />
    {% endif %}
  {% endfor %}
</div>
