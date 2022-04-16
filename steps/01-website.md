# 01 Build a website!

Your startup's ice-cream is super fresh and your website should be just as fresh 🍉.

Spin up a basic website and use this as your landing page:


```html
<!doctype html>
<html>
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Chakra+Petch:ital,wght@0,300;0,400;0,500;0,600;0,700;1,300;1,400;1,500;1,600;1,700&display=swap" rel="stylesheet">
    <script src="https://cdn.tailwindcss.com?plugins=forms,typography,aspect-ratio,line-clamp"></script>
    <script>
      tailwind.config = {
        theme: {
          extend: {
            colors: {
              chocolate: '#3f000f',
            }
          },
          borderRadius: {
            lg: '18px'
          },
        }
      };
    </script>
    <style>
      h1, h2, h3, h4, h5, h6 {
        font-family: 'Chakra Petch', sans-serif;
      }
      body {
        font-family: 'Chakra Petch', sans-serif;
      }
    </style>
  </head>
  <body>
    <div class="bg-white">
      <div class="relative">
        <!-- Decorative image and overlay -->

        <!-- Navigation -->
        <header class="relative z-10">
          <nav aria-label="Top">
            <!-- Top navigation -->
            <div class="bg-chocolate">
              <div class="max-w-7xl mx-auto h-10 px-4 flex items-center justify-between sm:px-6 lg:px-8">
                <div class="flex items-center space-x-6">
                  <a href="#" class="text-sm font-medium hover:text-gray-100 text-gray-100">Sign in</a>
                  <a href="#" class="text-sm font-medium hover:text-gray-100 text-gray-100">Create an account</a>
                </div>
              </div>
            </div>

            <!-- Secondary navigation -->
            <div class="bg-teal-200 bg-white">
              <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
                <div>
                  <div class="h-16 flex items-center justify-between">
                    <!-- Logo (lg+) -->
                    <div class="hidden lg:flex-1 lg:flex lg:items-center">
                      <a href="#">
                        <span class="sr-only">Airborne Treats</span>
                        <img class="h-8 w-auto" src="https://tailwindui.com/img/logos/workflow-mark.svg?color=white" alt="">
                      </a>
                    </div>

                    <div class="flex-1 flex items-center justify-end">
                      <div class="flex items-center lg:ml-8">
                        <!-- Cart -->
                        <div class="ml-4 flow-root lg:ml-8 text-chocolate">
                          <a href="#" class="group -m-2 p-2 flex items-center">
                            <!-- Heroicon name: outline/shopping-bag -->
                            <svg class="flex-shrink-0 h-6 w-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" aria-hidden="true">
                              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M16 11V7a4 4 0 00-8 0v4M5 9h14l1 12H4L5 9z" />
                            </svg>
                            <span class="ml-2 text-sm font-medium">0</span>
                            <span class="sr-only">items in cart, view bag</span>
                          </a>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </nav>
        </header>
      </div>

      <main>
        <!-- Category section -->
        <section aria-labelledby="category-heading" class="pt-24 sm:pt-32 xl:max-w-7xl xl:mx-auto xl:px-8">
          <div class="px-4 sm:px-6 sm:flex sm:items-center sm:justify-between lg:px-8 xl:px-0">
            <h2 class="text-2xl font-extrabold tracking-tight text-gray-900">Shop by Flavor</h2>
          </div>

          <div class="mt-4 flow-root">
            <div class="-my-2">
              <div class="box-content py-2 relative h-80 overflow-x-auto xl:overflow-visible">
                <div class="absolute min-w-screen-xl px-4 flex space-x-8 sm:px-6 lg:px-8 xl:relative xl:px-0 xl:space-x-0 xl:grid xl:grid-cols-5 xl:gap-x-8">
                  <!-- PRODUCT -->
                  <div>
                    <div class="relative">
                      <div class="relative w-full h-72 rounded-lg overflow-hidden">
                        <img src="https://github.com/cjavilla-stripe/checkout-workshop/raw/main/assets/images/vanilla.jpeg" alt="Front of zip tote bag with white canvas, black canvas straps and handle, and black zipper pulls." class="w-full h-full object-center object-cover">
                      </div>
                      <div class="relative mt-4">
                        <h3 class="text-sm font-medium text-gray-900">Vanilla</h3>
                        <p class="mt-1 text-sm text-gray-500">Tasty tasty tasty</p>
                      </div>
                      <div class="absolute top-0 inset-x-0 h-72 rounded-lg p-4 flex items-end justify-end overflow-hidden">
                        <div aria-hidden="true" class="absolute inset-x-0 bottom-0 h-36 bg-gradient-to-t from-black opacity-50"></div>
                        <p class="relative text-lg font-semibold text-white">$1</p>
                      </div>
                    </div>
                    <div class="mt-6">
                      <a href="#" class="relative flex bg-gray-100 border border-transparent rounded-md py-2 px-8 items-center justify-center text-sm font-medium text-gray-900 hover:bg-gray-200">Add to cart</a>
                    </div>
                  </div>
                  <!-- END PRODUCT -->

                  <!-- PRODUCT -->
                  <div>
                    <div class="relative">
                      <div class="relative w-full h-72 rounded-lg overflow-hidden">
                        <img src="https://github.com/cjavilla-stripe/checkout-workshop/raw/main/assets/images/chocolate.jpeg" alt="Front of zip tote bag with white canvas, black canvas straps and handle, and black zipper pulls." class="w-full h-full object-center object-cover">
                      </div>
                      <div class="relative mt-4">
                        <h3 class="text-sm font-medium text-gray-900">Chocolate</h3>
                        <p class="mt-1 text-sm text-gray-500">Yummy yummy yummy</p>
                      </div>
                      <div class="absolute top-0 inset-x-0 h-72 rounded-lg p-4 flex items-end justify-end overflow-hidden">
                        <div aria-hidden="true" class="absolute inset-x-0 bottom-0 h-36 bg-gradient-to-t from-black opacity-50"></div>
                        <p class="relative text-lg font-semibold text-white">$1</p>
                      </div>
                    </div>
                    <div class="mt-6">
                      <a href="https://buy.stripe.com/test_00g9BX1vOf7AgA8aEE" class="relative flex bg-gray-100 border border-transparent rounded-md py-2 px-8 items-center justify-center text-sm font-medium text-gray-900 hover:bg-gray-200">Buy</a>
                    </div>
                  </div>
                  <!-- END PRODUCT -->

                </div>
              </div>
            </div>
          </div>
        </section>
      </main>
    </div>
  </body>
</html>
```

Take a look around, checkout the medicine cabinets, see if there are any spots
on the silverware 🥄. Feel free to tweak a bit to make it your own.

For now, we'll just keep using Payment Links on each product, but Cherry isn't going to
be okay with this for long. We learned at work that we can do this thing called
"fast follow" after GA, so we'll just tell Cherry that.


### Actions

Set up your page so that it fetches the flavors from inventory. At the end of
this section you should have a simple index page rendering all of the flavors.
No need to actually implement Checkout, yet.


Ideas:

* Pull from the Stripe API
* Hard code some client side JSON
* Retrieve from a database and use SSR
* Render back JSON from a server side endpoint


🧠 What are the tradeoffs with each of those approaches? What data do you
_really_ need for display? What about data required for ultimately [creating the
Checkout Session](https://stripe.com/docs/api/checkout/sessions/create)?


---

[<- Back to 00 Add products](./00-add-products.md)
|
[Next O2 Flavor selection ->](./02-flavor-selection.md)


[TODO](../TODO.md)
