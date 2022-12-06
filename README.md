# python2project
#multiple in heritance
#multiple inheritance :-in this a single class will take the features from multiple base classes.
class student:   # base class 1
    def getinfo(self,r,n):
        self.r=r
        self.n=n
    def printinfo(self):
        print(self.r,self.n)

class sports: #base class 2
    def getsports(self,interest):
        self.interest=interest
    def printsports(self):
        print(self.interest)


class result (student,sports): #derived
    def getmarks(self,marks):
        self.marks=marks
    def printmarks(self):
        print(self.marks)

r=result()
r.getinfo(1,'abc')
r.getsports('cricket')
r.getmarks(456)
r.printinfo()
r.printsports()
r.printmarks()
