#lang racket

(define a 42)             ;(1) atribuir 42 a variável 'a'

(define b 14)             ;(2) atribuir 14 a variável 'b'

(+ a b)                   ;(3.1) somar
(- a b)                   ;(3.2) subtrair
(+ a (* 3 b) 7)           ;(3.3) somar e multiplicar números e variáveis
(/ (+ a b) 2)             ;(3.4) média aritmética
(sqrt (* a b))            ;(3.5) média geométrica
(/ 2 (+ (/ 1 a) (/ 1 b))) ;(3.6) média harmônica

(  define soma-medias ( + (/ (+ a b) 2) (/ 2 (+ (/ 1 a) (/ 1 b))) )  ) ;(4) somar (3.4) e (3.6)

(if (= soma-medias 49) "teste 1 ok" "teste 1 falhou") ;(5) testar se soma-medias é igual a 49

(define (quadrado num)    ;(6) criar função quadrado para receber um número qualquer
  (* num num)
)

(define (delta a b c)     ;(7) reecrever função delta e raiz-positiva vista na aula, usando função quadrado
  (- (quadrado b) (* 4 a c))
)

(define (raiz-positiva a b c)
  (/ (+ (- b) (sqrt (delta a b c))) (* 2 a))
)

(define (potencia x y) 
  ;é um número inteiro?
  (if (exact? y)
      (if (= y 0)
          1
          ;senao faça as contas
          (if (> y 0)
              ;true
              (if (= y 1)
                  ;true: x
                  x
                  ;false: recursivamente 
                  (* x (potencia x (- y 1)))
              )
              ;false
              (if (= y -1)
                  ;true: x
                  ""
                  ;false:
                  ""
               )
          )
      )
      ;false: y não é inteiro
      "a potência y não é um número inteiro"
   )
)

(define (potencia1 x y)
  ;é um número inteiro?
  (if (exact? y)
      "a potência y não é um número inteiro"
      "teste"
  )
)