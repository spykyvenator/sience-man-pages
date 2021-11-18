# sience Man pages

## Tools
	units: tool for converting units on the command line
	groff: converting text to man pages

##handy man pages:
	man groff
	man eqn => format math equations for troff and groff

## Rules
	variables should be declared after the formula like this, if not it should be treated as a Real number:
		x=e^(i*pi)+1
		where x = 0, e = Eulers number, pi = 3.1415 and i = imaginary unit
	
	all units should be of the SI format, so no yards, miles etc
	temperature should be in Kelvin, but references to the other systems should be made when these are convenient:
		Water freezes under 273.15 K or 0 degrees Celsius
		the human body temperature averages around 308 K or 96 degrees fahrenheit

## usage (make script)
		move text files to /usr/local/man/man7/ -> sudo mv ./sience /usr/local/man/man7/sience.7
		compress with gzip -> sudo gzip /usr/local/man/man7/sience.7
		view with groff -> groff -Tascii -man ./file | more
