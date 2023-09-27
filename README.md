# if
funcionarios = []

# name
20.times do |i|
  puts "Digite o nome do funcionário #{i + 1}:"
  nome = gets.chomp

  puts "Digite o salário de #{nome}:"
  salario = gets.to_f

  # Calcule o novo salário com o reajuste de 8%
  novo_salario = salario * 1.08

  funcionario = { nome: nome, salario: salario, novo_salario: novo_salario }
  funcionarios << funcionario
end

# print
puts "\nListagem de funcionários com os novos salários:"
funcionarios.each do |funcionario|
  puts "Nome: #{funcionario[:nome]}, Novo Salário: #{funcionario[:novo_salario]}"
end
