# Proje1-2
Patika.dev projesi kapsamında yapmış olduğum 2 Proje

## Proje 1 - Verilen Listeyi Düz bir listeye dönüştürüyoruz.

flatten_list = []
def flatten(l):
    for i in l:
        if type(i) == list:
            flatten(i)
        else:
            flatten_list.append(i)
    return flatten_List
    l = [[1,'a',['cat'],2],[[[3]],'dog'],4,5]
    flatten(l)
    
## Proje 2 - Verilen listenin elemanlarını tersine çeviriyoruz.
def reverser(x):
    x.reverse()
    for i in x:
        if type(i) == list:
            reverser(i)
exp_list=[[1, 2], [3, 4], [5, 6, 7]]
reverser(exp_list)
print(exp_list)
