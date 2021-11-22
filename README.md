# SASS CSS NOTES

## INSTALLING

1. npm install -g sass
2. LIVE SAAS COMPILER WIDGET for VSCODE
3. [VISIT FOR MORE INFO](https://sass-lang.com/install)

---

## VARIABLES

### EXAMPLES

$list-border: solid 3px $primary-color;
$primary-color:red;
p{
color:$primary-color;
border: $list-border;
}

## MAP USAGE

$margin-map(m1:1rem, m2:2rem, m3:3rem);
li {
margin:map-get($margin-map,m1);
}

## & USAGE

li {
color:$primary-color;
&:hover{
color:white;
}
}

## MIXIN USAGE

MIXIN USED FOR NESTED SFECIFIC CONTENT a ELEMENT EXC.

@mixin main-a($mcolor: red, $hcolor: black) {
text-decoration: none;
color: $mcolor;
&:hover {
color: $hcolor;
}
}

a{
@include main-a(navy, white);
}
