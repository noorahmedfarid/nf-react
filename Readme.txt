Atomic Design
Atoms: Basic building blocks
Molecues: Groups of two or more atoms
Organisms: Groups of molecules funcitioning together

Atom: Prgress bar label and image
Smallest building block
The foundation of a component library
Typically composed together

Submit, save cancel save as
It is small , it can not break, single responsibility
Wrap HTML Primitives Enhancement:

<cash>6</cash>  $6
<Cash showDecimal={false}>6.23</Cash> $6

Progress bar: change color based on percentage change
Label: with optional field marker
icon: SVG
Requirement:
1. Vertical form layout
2. Mark required fields with red asterisk
3. Apply htmlFor to associate label to input for accessibility

Pass props via spreed
Use spreed with destructuring

Molecule: 
Should have also have a single (but higher level) responsibility. Encapsulate opinions
Atom are combined with specific purpose(to achieve consistency and reduce decision fatigue)
-TextInput
	Integrated label
	Associated label to input
	Required field indicator
	Enforced layout
-PasswordInput
	Display password quality
	Toggle passward visibility
	It is a specialization of the TextInput
	Composition over Inheritence 
Consist of following:
label, OnChange, maxLength, minLength, placeholder, show visibilityToggle, and Quality

What remain Flexible and what remain Fixed.

Organism:
Strong opinion are a feature and keep organisms dumb. higher-level patterns with Facade
Strive to limit the props that we expose from our underlying components
Use Containers to save people time
Take inputs/parameters and return HTML

-RegistrationForm




