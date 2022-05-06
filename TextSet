
def initData(dataStr):
    # print(dataStr)
    set_ = set(dataStr.split("\n"))

    # print("XXXXXXXXXXXXXXXXXXXXX")
    # for xx in set_:
    #     print(len(xx), xx)
    #     # print(len(xx), ord(xx[0]), xx)
    # print("XXXXXXXXXXXXXXXXXXXXX")


    set_.add('')
    set_.remove('')
    # set_.add("\t")
    # set_.remove("\t")
    # set_.add("    ")
    # set_.remove("    ")
    # set_.add("\n")
    # set_.remove("\n")
    return set_


def test_load(listA, listB):
    setA = initData(listA)
    setB = initData(listB)

    output("Set A", setA)
    output("Set B", setB)

    output("A - B", setA.difference(setB))
    output("B - A", setB.difference(setA))
    output("A and B", setA.intersection(setB))
    output("A or B", setA.union(setB))
    output("(A or B) - (A and B)", setA.symmetric_difference(setB))


def output(msg, dataSet):
    print("###########", msg, "################\t//")
    list_ = list(dataSet)
    list_.sort()
    print(*list_, sep='\n')


############################
import sys

__debug = False
# __debug = True
if __debug is True:
    print("============== DEBUG ===================+======")
    try:
        print("arg len : ", len(sys.argv))
        print("arg 1 : ", (sys.argv[1]))
        print("arg 2 : ", (sys.argv[2]))
    except:
        None
    print("============== DEBUG ===================+======")

if len(sys.argv) == 1 or sys.argv[1] == "":
    print("No args... by Test Data")
    listA = '''
bb
cc
aa
'''
    listB = '''
cc
dd
ee
'''
    sys.argv.append("dummy...")
    sys.argv.append("dummy...")
    sys.argv[1] = listA
    sys.argv[2] = listB

test_load(sys.argv[1], sys.argv[2])
