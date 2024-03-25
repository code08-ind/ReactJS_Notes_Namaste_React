# Jo Dikhta Hai Vo Bikta Hai

We can add our styles using:
1. Styled Components
2. SASS, SCSS.
3. CSS
4. Material UI
5. Tailwind CSS
6. Bootstrap
7. Chakra UI
8. Ant Design

tailwind.config.css: This file is used to configure the tailwind CSS. It will include the content on which we can include our tailwind css.
.postcssrc: This is the configuration for postcss in our system and we will tell it to use tailwind css as our css processor.

@tailwind ...: This is used to import tailwind into our application. We can also add various of the different classes here into our application.

align-items: This will align the items in y-axis and justify-content will be used to align the items in x-axis.

If we don't have a class predefined in tailwind css, we can add our own class in the tailwind by using w-[200px] and it will take it as size for that component where we define the class inside here.

We can use tailwind-ui pre made components here itself. One con for this is that we are having many classes that are attached inside the system here into the classnames here inside our tag and code readability decreases a lot here.

Tailwind CSS is a utility-first CSS framework for rapidly building custom designs. It is a low-level framework that provides a lot of utility classes that can be used to build custom designs. It is a highly customizable framework that allows you to build designs without writing any CSS code. It is very lightweight and it will only include the css that will be used here with us and it will include css that is used into our application and not the whole css classes we have given into our application and it will be really benefitial in the bundling of our application here.

We can also add hover classes as well using tailwindcss into our application.

It will only add the the css classes that are necessary to be added or are used and it will remove the css classes that are not to be added up or are not to be used by the user.

We can also give styles for different screen sizes we will be using up here.

Nowadays we also require theme for our applications, so we now can use dark theme easily with tailwindcss.
