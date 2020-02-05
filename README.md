users = {}

while True:
  create_username = input('Please submit your username: ')
  if create_username == '':
    break

  if create_username in users:
    submit_password = input('Please enter your password: ')
  else: 
    create_password = input('Please create a password that you can remember: ')
    users[create_username] = create_password
    break

print(users)
