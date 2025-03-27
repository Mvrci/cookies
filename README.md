# CALCULATOR

def sprawdzanie_liczby():
    liczba1 = sprawdzanie_czy_liczba()
    while liczba1 is None:
        liczba1 = sprawdzanie_czy_liczba()
    return liczba1

def sprawdzanie_czy_liczba():
    try:
        liczba1 = int(input("Podaj liczbę: "))
        return liczba1
    except:
        print("Podano złą liczbę")
        return

def kalkulator():
    liczba1 = sprawdzanie_liczby()
    liczba2 = sprawdzanie_liczby()
    # if liczba1 is None or liczba2 is None:
    #     print("Nie mogę wykonać zadania")
    #     return
    obliczanie(liczba1, liczba2)

def obliczanie(x1, x2):

    obliczanie = input("Co chcesz zrobić z tymi liczbami? (+, -, *, /) ")
    if obliczanie == "+":
        print(x1 + x2)
    elif obliczanie == "-":
        print(x1 - x2)
    elif obliczanie == "*":
        print(x1 * x2)
    elif obliczanie == "/":
        print(x1 / x2)
    else:
        print("Upewnij się, że wpisałeś poprawny znak")



kalkulator()
