# PracticaBDD
Desarrollo de la kata FizzBuzz mediante BBD
Siguiendo el tutorial de la página https://www.pmareke.com/posts/bdd-in-python/

Se corrige error existente en el tutorial.
en la fase refactor indica :
=============================================================
en el fichero .feature
=============================================================
      Feature: FizzBuzz
          Scenario: FizzBuzz for number 3
              Given the number "3"
              When calculates the result
              Then the result should be "Fizz"

=============================================================
en el fichero steps.py
=============================================================
@given('the number "{number}"')
def number(context, number):
    context.number = number 

Se corrige el @given la linea context.number = number se cambia por context.number = int(number)
