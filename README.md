class Bag:

    def __init__(self):

        self.TheItems = list()





    def __len__(self):

        return len(self.TheItems)



    def __contains__(self, item):

        return item in self.TheItems





    def add(self,item):

        self.TheItems.append(item)



    def remove(self,item):

        assert item in self.TheItems

        ndx = self.TheItems.index(item)

        return self.TheItems.pop(ndx)





    def __iter__(self):

        return BagIteretor(self.TheItems)



class BagIteretor:

    def __init__(self,theList):

        self.bagItems = theList

        self.curItem = 0





    def __iter__(self):

        return self





    def __next__(self):

        if self.curItem < len(self.bagItems):

            item = self.bagItems(self.curItem)

            self.curItem +=1

            return item

        else:

            raise StopIteration



b1 = Bag()



b1.add("kaan")

b1.add("rli")

b1.add(12)

b1.add(89)





print(b1.__len__())

print(b1.__contains__("kaan"))

b1.remove("kaan")



print(b1.__contains__("kaan"))



