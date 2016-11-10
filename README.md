# cljs-exponent

[Exponent.js](https://getexponent.com/) clojurescript binding.

## Usage

### Api

``` clojure
(require '[cljs-exponent.contacts :as contacts])

(contacts/get-contacts-async [(aget contacts/Contacts "PHONE_NUMBER")
                              (aget contacts/Contacts "EMAIL")])
```

### Components
Supports both [Om](https://github.com/omcljs/om) and [Reagent](https://github.com/reagent-project/reagent).

#### Om

``` clojure
(require '[cljs-exponent.om :as ex])

(ex/linear-gradient
 {:colors ["#4c669f" "#3b5998" "#192f6a"]
  :style {:padding 15
          :alignItems "center"
          :borderRadius 5}}
 (text {:style {:backgroundColor "transparent"
                :fontSize 15
                :color "#fff"}}
   "Sign in with Facebook"))
```

#### Reagent

``` clojure
(require '[cljs-exponent.reagent :as ex])

[ex/linear-gradient
 {:colors ["#4c669f" "#3b5998" "#192f6a"]
  :style {:padding 15
          :align-items "center"
          :border-radius 5}}
 [text {:style {:background-color "transparent"
                :font-size 15
                :color "#fff"}}
  "Sign in with Facebook"]]
```

## License

Copyright © 2016 tiensonqin@gmail.com

Distributed under the Eclipse Public License either version 1.0 or (at
your option) any later version.