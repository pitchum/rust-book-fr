<!--
## Appendix A: Keywords
-->

## Annexe A : les mots-clés

<!--
The following list contains keywords that are reserved for current or future
use by the Rust language. As such, they cannot be used as identifiers (except
as raw identifiers as we’ll discuss in the “[Raw
Identifiers][raw-identifiers]<!-- ignore -- >” section), including names of
functions, variables, parameters, struct fields, modules, crates, constants,
macros, static values, attributes, types, traits, or lifetimes.
-->

La liste suivante contient des mots-clés réservés qui sont actuellement
utilisés dans le langage Rust ou qui pourraient l'être à l'avenir. De ce fait, 
ils ne peuvent pas être utilisés comme identificateurs (sauf comme identificateurs bruts, ce que
nous allons voir dans la section
“[les identificateurs bruts][raw-identifiers]<!-- ignore -->”), y compris pour les
noms de fonctions, de variables, de paramètres, de champs de structures, de
modules, de crates, de constantes, de macros, de valeurs statiques, d'attributs,
de types, de traits ou de durées de vie.

<!--
[raw-identifiers]: #raw-identifiers
-->

[raw-identifiers]: #les-identificateurs-bruts

<!--
### Keywords Currently in Use
-->

### Les mots-clés actuellement utilisés

<!--
The following keywords currently have the functionality described.
-->

Les mots-clés suivants ont actuellement la fonction décrite.

<!--
* `as` - perform primitive casting, disambiguate the specific trait containing
  an item, or rename items in `use` and `extern crate` statements
* `async` -  return a `Future` instead of blocking the current thread
* `await` - suspend execution until the result of a `Future` is ready
* `break` - exit a loop immediately
* `const` - define constant items or constant raw pointers
* `continue` - continue to the next loop iteration
* `crate` - link an external crate or a macro variable representing the crate in
  which the macro is defined
* `dyn` - dynamic dispatch to a trait object
* `else` - fallback for `if` and `if let` control flow constructs
* `enum` - define an enumeration
* `extern` - link an external crate, function, or variable
* `false` - Boolean false literal
* `fn` - define a function or the function pointer type
* `for` - loop over items from an iterator, implement a trait, or specify a
  higher-ranked lifetime
* `if` - branch based on the result of a conditional expression
* `impl` - implement inherent or trait functionality
* `in` - part of `for` loop syntax
* `let` - bind a variable
* `loop` - loop unconditionally
* `match` - match a value to patterns
* `mod` - define a module
* `move` - make a closure take ownership of all its captures
* `mut` - denote mutability in references, raw pointers, or pattern bindings
* `pub` - denote public visibility in struct fields, `impl` blocks, or modules
* `ref` - bind by reference
* `return` - return from function
* `Self` - a type alias for the type we are defining or implementing
* `self` - method subject or current module
* `static` - global variable or lifetime lasting the entire program execution
* `struct` - define a structure
* `super` - parent module of the current module
* `trait` - define a trait
* `true` - Boolean true literal
* `type` - define a type alias or associated type
* `union` - define a [union] and is only a keyword when used in a union declaration
* `unsafe` - denote unsafe code, functions, traits, or implementations
* `use` - bring symbols into scope
* `where` - denote clauses that constrain a type
* `while` - loop conditionally based on the result of an expression
-->

* `as` - effectue une transformation de type primitive, précise le trait qui contient un
  élément ou renomme des éléments dans les instructions `use` et `extern crate`
* `async` - retourne un `Future` plutôt que de bloquer la tâche en cours
* `await` - met en pause l'exécution jusqu'à ce que le résultat d'un `Future`
  soit disponible
* `break` - sort immédiatement d'une boucle
* `const` - définit des éléments constants ou des pointeurs bruts constants
* `continue` - passe directement à la prochaine itération de la boucle en cours
* `crate` - crée un lien vers une crate externe ou une variable de macro qui
  représente la crate dans laquelle la macro est définie
* `dyn` - utilisation dynamique d'un objet trait
* `else` - une branche de repli pour les structures de contrôle de flux `if`
  et `if let`
* `enum` - définit une énumération
* `extern` - crée un lien vers une crate, une fonction ou une variable externe
* `false` - le littéral qui vaut “faux” pour un booléen
* `fn` - définit une fonction ou le type pointeur de fonction
* `for` - crée une boucle sur les éléments d'un itérateur, implémente un trait,
  ou renseigne une durée de vie de niveau supérieur
* `if` - une branche liée au résultat d'une expression conditionnelle
* `impl` - implémente des fonctionnalités propres à un élément ou à un trait
* `in` - fait partie de la syntaxe de la boucle `for`
* `let` - lie une valeur à une variable
* `loop` - fait une boucle sans condition (théoriquement infinie)
* `match` - compare une valeur à des motifs
* `mod` - définit un module
* `move` - fait en sorte qu'une fermeture prenne possession de tout ce qu'elle
  utilise
* `mut` - autorise la mutabilité sur des références, des pointeurs bruts ou des
  éléments issus de motifs
* `pub` - autorise la visibilité publique sur des champs de structures, des
  blocs `impl` ou des modules
* `ref` - lie une valeur avec une référence
* `return` - retourne une valeur depuis une fonction
* `Self` - un alias de type pour le type que nous définissons ou implémentons
* `self` - désigne le sujet d'une méthode ou du module courant
* `static` - une variable globale ou une durée de vie qui persiste tout au long de
  l'exécution du programme
* `struct` - définit une structure
* `super` - le module parent du module courant
* `trait` - définit un trait
* `true` - le littéral qui vaut “vrai” pour un booléen
* `type` - définit un alias de type ou un type associé
* `union` - définit une [union] mais n'est un mot-clé que lorsqu'il est utilisé
  dans la déclaration d'une union
* `unsafe` - autorise du code, des fonctions, des traits ou des implémentations
  non sécurisées
* `use` - importe des éléments dans la portée
* `where` - indique des conditions pour contraindre un type
* `while` - crée une boucle en fonction des résultats d'une expression

<!--
[union]: ../reference/items/unions.html
-->

[union]: https://doc.rust-lang.org/reference/items/unions.html

<!--
### Keywords Reserved for Future Use
-->

### Les mots-clés réservés pour une utilisation future

<!--
The following keywords do not have any functionality but are reserved by Rust
for potential future use.
-->

Les mots-clés suivants n'offrent actuellement aucune fonctionnalité mais sont
réservés par Rust pour une potentielle utilisation future.

<!--
* `abstract`
* `become`
* `box`
* `do`
* `final`
* `macro`
* `override`
* `priv`
* `try`
* `typeof`
* `unsized`
* `virtual`
* `yield`
-->

* `abstract`
* `become`
* `box`
* `do`
* `final`
* `macro`
* `override`
* `priv`
* `try`
* `typeof`
* `unsized`
* `virtual`
* `yield`

<!--
### Raw Identifiers
-->

### Les identificateurs bruts

<!--
*Raw identifiers* are the syntax that lets you use keywords where they wouldn’t
normally be allowed. You use a raw identifier by prefixing a keyword with `r#`.
-->

Un *identificateur brut* est une syntaxe qui vous permet d'utiliser des
mots-clés là où ils ne devraient pas pouvoir l'être. Vous pouvez utiliser un
identificateur brut en faisant précéder un mot-clé par un `r#`.

<!--
For example, `match` is a keyword. If you try to compile the following function
that uses `match` as its name:
-->

Par exemple, `match` est un mot-clé. Si vous essayez de compiler la fonction
suivante qui utilise `match` comme nom :

<!--
<span class="filename">Filename: src/main.rs</span>
-->

<span class="filename">Fichier : src/main.rs</span>

<!--
```rust,ignore,does_not_compile
fn match(needle: &str, haystack: &str) -> bool {
    haystack.contains(needle)
}
```
-->

```rust,ignore,does_not_compile
fn match(aiguille: &str, botte_de_foin: &str) -> bool {
    botte_de_foin.contains(aiguille)
}
```

<!--
you’ll get this error:
-->

… vous allez obtenir l'erreur suivante :

<!--
```text
error: expected identifier, found keyword `match`
 -- > src/main.rs:4:4
  |
4 | fn match(needle: &str, haystack: &str) -> bool {
  |    ^^^^^ expected identifier, found keyword
```
-->

```text
error: expected identifier, found keyword `match`
 -- > src/main.rs:4:4
  |
4 | fn match(aiguille: &str, botte_de_foin: &str) -> bool {
  |    ^^^^^ expected identifier, found keyword
```

<!--
The error shows that you can’t use the keyword `match` as the function
identifier. To use `match` as a function name, you need to use the raw
identifier syntax, like this:
-->

L'erreur montre que vous ne pouvez pas utiliser le mot-clé `match` comme
identificateur de la fonction. Pour utiliser `match` comme nom de fonction, vous
devez utiliser la syntaxe d'identificateur brut, comme ceci :

<!--
<span class="filename">Filename: src/main.rs</span>
-->

<span class="filename">Fichier : src/main.rs</span>

<!--
```rust
fn r#match(needle: &str, haystack: &str) -> bool {
    haystack.contains(needle)
}

fn main() {
    assert!(r#match("foo", "foobar"));
}
```
-->

```rust
fn r#match(aiguille: &str, botte_de_foin: &str) -> bool {
    botte_de_foin.contains(aiguille)
}

fn main() {
    assert!(r#match("rem", "lorem ipsum"));
}
```

<!--
This code will compile without any errors. Note the `r#` prefix on the function
name in its definition as well as where the function is called in `main`.
-->

Ce code va se compiler sans erreur. Remarquez le préfixe `r#` sur le nom de la
fonction dans sa définition mais aussi lorsque cette fonction est appelée dans
`main`.

<!--
Raw identifiers allow you to use any word you choose as an identifier, even if
that word happens to be a reserved keyword. In addition, raw identifiers allow
you to use libraries written in a different Rust edition than your crate uses.
For example, `try` isn’t a keyword in the 2015 edition but is in the 2018
edition. If you depend on a library that’s written using the 2015 edition and
has a `try` function, you’ll need to use the raw identifier syntax, `r#try` in
this case, to call that function from your 2018 edition code. See [Appendix
E][appendix-e]<!-- ignore -- > for more information on editions.
-->

Les identificateurs bruts vous permettent d'utiliser n'importe quel mot de votre choix
comme identificateur, même si ce mot est un mot-clé réservé. De plus,
les identificateurs bruts vous permettent d'utiliser des bibliothèques écrites
dans des éditions de Rust différentes de celle qu'utilise votre crate. Par
exemple, `try` n'est pas un mot-clé dans l'édition 2015, mais il l'est dans
l'édition 2018. Si vous dépendez d'une bibliothèque qui était écrite avec
l'édition 2015 et qui avait une fonction `try`, vous allez avoir besoin dans ce cas
d'utiliser la syntaxe d'identificateur brut `r#try` pour faire
appel à cette fonction à partir de code écrit avec l'édition 2018. Voir
[l'annexe E][appendix-e]<!-- ignore --> pour en savoir plus sur les éditions.

<!--
[appendix-e]: appendix-05-editions.html
-->

[appendix-e]: appendix-05-editions.html
