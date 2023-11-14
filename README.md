import pickle

name_file = "user.dat"
order1 = [
    {1: 'choclate'},
    {2: 'bread'},
    {3: "milk"},
]
order2 = [
    {1:'hamburger'},
    {2: 'sweet'},
    {3:"water"},
]
with open(name_file, "wb") as file:
    pickle.dump(order1, file)
    pickle.dump(order2, file)

with open(name_file, "rb") as file:
    orders_file = pickle.load(file)
