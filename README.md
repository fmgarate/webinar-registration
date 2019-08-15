# webinar-registration

This demo project shows the use of optional named slots on Vue js.
The `WebinarRegistration` component can be used with a header or footer slots.

### Simple example - Default content
``` html
<webinar-registration />
```

The rendered components structure is:
``` html
<WebinarRegistration>
  <WebinarRegistrationForm />
</WebinarRegistration>
```

### Complete example - Header and footer content
``` html
<webinar-registration>
  <template v-slot:header>
    <h1>
      Welcome to this masterclass
    </h1>
  </template>
  <template v-slot:footer>
    <p>
      Lorem ipsum dolor sit amet, consectetur adipisicing elit
    </p>
  </template>
</webinar-registration>
```

The rendered components structure is:
``` html
<WebinarRegistration>
  <div class="webinar-registration-header" />
  <WebinarRegistrationForm />
  <div class="webinar-registration-footer" />
</WebinarRegistration>
```

## Build Setup

``` bash
# install dependencies
$ npm run install

# serve with hot reload at localhost:3000
$ npm run dev

# build for production and launch server
$ npm run build
$ npm run start

# generate static project
$ npm run generate
```

For detailed explanation on how things work, check out [Nuxt.js docs](https://nuxtjs.org).
