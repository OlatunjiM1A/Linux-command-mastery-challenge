# Day 27 Practice Drill

## Task
Generate an SSH key pair, copy the public key to a remote host, connect
without a password, then securely copy a file to and from that server.

## Commands run, in order

ssh-keygen -t ed25519 -C "day27"
ssh-copy-id ubuntu@32.199.184.245
ssh ubuntu@32.199.184.245
exit
echo "Hello from WSL to AWS" > test_upload.txt
scp test_upload.txt ubuntu@32.199.184.245:~/
scp ubuntu@32.199.184.245:~/test_upload.txt ./downloaded_from_aws.txt
