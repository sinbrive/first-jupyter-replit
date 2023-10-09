# Jupyter on Replit

Create Jupyter notebooks on Replit!

Instructions:

1. In the shell run `./generate_password.sh`
2. Enter password for your Jupyter notebook.
3. Copy enecrypted password to a Replit Secret with the name `NOTEBOOK_PASSWORD`
4. Run the repl
5. Open the webview in a new tab (you cannot log in via the webview in the workspace)
6. Log in with the password you entered in step 2

Add package in Replit.nix

<pre>{ pkgs }: {
	deps = [
		pkgs.jupyter
    pkgs.jq
    pkgs.python3
    pkgs.python3Packages.pip
    pkgs.python3Packages.pandas
    pkgs.python3Packages.numpy
    pkgs.python3Packages.flask
    pkgs.python3Packages.matplotlib
        pkgs.python3Packages.pylab 
	];
}</pre>

test_new_package_nix

![image](https://github.com/sinbrive/first-jupyter-replit/assets/21102151/5d3b7a0c-db20-4eb7-ab4e-6afb51308921)

