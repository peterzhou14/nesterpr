# nesterpr
# A printer of nested lists by Python
'''This is the "nesterpr.py" module and it provides one function called
"print_pr()" which prints lists that may or may not include nested lists.'''

def print_pr(the_list):
    '''This function takes one positional argument called "the_list", which is
any Python list(of-possibly-nested lists). Each data item in the provided list
is printed (recursively) to the screen on its own line.'''
    for each_item in the_list:
        if isinstance(each_item,list):
            print_pr(each_item)
        else:
            print(each_item)
