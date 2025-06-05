def contiene_solo_mayus(txt):
    vm = False

    for l in txt:
        if (l >= "A") and (l <= "Z"):
            vm = True

        elif (l >= "a") and (l <= "z"):

            return False
    return vm

def contiene_dig(text):

    vn = False

    for num in text:

            if (num >= "0") and (num <= "9"):

                vn = True
    return vn


def validar_numero_orden(nc):

    validez = True

    if nc == "":
        validez = False

    elif not(contiene_solo_mayus(nc) or contiene_dig(nc)) and "-" in nc or not(contiene_solo_mayus(nc)):
        validez = False

    return validez
