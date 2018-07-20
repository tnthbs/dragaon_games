# dragaon_games
#！python 3
usrinv = {'rope':1,'torch':6,'gold coin':42,'dagger':1,'arrow':12}
dragonLoot =['gold coin','dagger','gold coin','gold coin','ruby','sword']


def displayInventory(inventory): #print the item and numbers of user inventory
    total = 0
    print('Inventory')
    for k,v in inventory.items():
        print(str(v) + ' ' +str(k))
        total = total + v
    print('Total number of items: ' + str(total))
    

def addInventory(inventory,addItmes):
    for i in addItmes:
        if i in inventory: #若已有key，value = value +1
            inventory[i] += 1
        else:               #若没有键，新增加key,value =1
            inventory[i] = 1


displayInventory(usrinv)
addInventory(usrinv,dragonLoot)
displayInventory(usrinv)
