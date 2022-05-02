
# Install it with the following commands:

sudo apt-get update
sudo apt-get install ssmtp

Edit /etc/ssmtp/ssmtp.conf to look like this:

root=rpi3abc@gmail.com
mailhub=smtp.gmail.com:465
FromLineOverride=YES
AuthUser=rpi3abc@gmail.com
AuthPass=testing123
UseTLS=YES


# Send a one-liner like so:

echo "Testing...1...2...3" | ssmtp myusername@gmail.com

# url

https://unix.stackexchange.com/questions/363814/simplest-way-to-send-one-line-mail-out-via-command-line-using-gmail
