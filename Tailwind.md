step-1: npm install -D tailwindcss

step-2: npx tailwindcss init

"-step-3: Create folder inside create a file style.css
@import 'tailwindcss/base';
@import 'tailwindcss/components';
@import 'tailwindcss/utilities';

@import 'app/header.scss';
@import 'app/footer.scss "

"-step-4: Edit package.json
"scripts":
{
"dev":"tailwind build -i src/style.css -o dist/style.css",
"prod":"tailwind build -i src/style.css -o dist/style.css --minify",
"watch":"tailwind build -i src/style.css -o dist/style.css --watch"
},"

"-step-5: Edit tailwind.config.js file inside to content Array
content: ['./dist/**/*.{html,js}'],"

"-step-6: Link in css style file inside html

<link rel="stylesheet" href="style.css" />"

step-7: every style added than command on
"npm rum dev/prod/watch"
