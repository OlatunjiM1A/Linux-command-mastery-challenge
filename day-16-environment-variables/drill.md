# Day 16 Practice Drill

## Task
Set a temporary environment variable, confirm it exists, unset it, then
add a directory to your PATH for the current session only and prove the
shell can now find a script inside it.

## Commands run, in order

export MYVAR="test123"
echo $MYVAR
unset MYVAR
echo $MYVAR
mkdir -p ~/myscripts
echo 'echo "Script ran successfully"' > ~/myscripts/hello.sh
chmod +x ~/myscripts/hello.sh
export PATH=$PATH:~/myscripts
hello.sh
