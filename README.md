<div class="text-white">
  <h3 class="text-lg font-medium">Saldo Disponível:</h3>
  <p class="text-2xl font-bold">3500.00000000 BTC</p>
</div>

<!-- Nome do Banco -->
<div>
  <label for="bank-name" class="block text-sm font-medium text-gray-400">Nome do Banco</label>
  <input type="text" id="bank-name" name="bank-name" class="mt-1 bg-gray-800 block w-full pl-3 pr-10 py-2 text-base text-white font-bold border-gray-700 focus:outline-none focus:ring-blue-500 focus:border-blue-500 sm:text-sm rounded-md" placeholder="Ex: Banco do Brasil">
</div>

<!-- CPF/CNPJ do Titular da Conta -->
<div>
  <label for="account-holder-cpf-cnpj" class="block text-sm font-medium text-gray-400">CPF/CNPJ do Titular da Conta</label>
  <input type="text" id="account-holder-cpf-cnpj" name="account-holder-cpf-cnpj" class="mt-1 bg-gray-800 block w-full pl-3 pr-10 py-2 text-base text-white font-bold border-gray-700 focus:outline-none focus:ring-blue-500 focus:border-blue-500 sm:text-sm rounded-md" placeholder="000.000.000-00">
</div>

<!-- Agência -->
<div>
  <label for="agency-number" class="block text-sm font-medium text-gray-400">Agência</label>
  <input type="text" id="agency-number" name="agency-number" class="mt-1 bg-gray-800 block w-full pl-3 pr-10 py-2 text-base text-white font-bold border-gray-700 focus:outline-none focus:ring-blue-500 focus:border-blue-500 sm:text-sm rounded-md" placeholder="0000">
</div>

<!-- Número da Conta -->
<div>
  <label for="account-number" class="block text-sm font-medium text-gray-400">Número da Conta</label>
  <input type="text" id="account-number" name="account-number" class="mt-1 bg-gray-800 block w-full pl-3 pr-10 py-2 text-base text-white font-bold border-gray-700 focus:outline-none focus:ring-blue-500 focus:border-blue-500 sm:text-sm rounded-md" placeholder="00000-0">
</div>

<!-- Tipo de Conta -->
<div>
  <label for="account-type" class="block text-sm font-medium text-gray-400">Tipo de Conta</label>
  <select id="account-type" name="account-type" class="mt-1 bg-gray-800 block w-full pl-3 pr-10 py-2 text-base text-white font-bold border-gray-700 focus:outline-none focus:ring-blue-500 focus:border-blue-500 sm:text-sm rounded-md">
    <option>Corrente</option>
    <option>Poupança</option>
  </select>
</div>

<!-- Quantia a Ser Sacada -->
<div>
  <label for="amount" class="block text-sm font-medium text-gray-400">Quantia</label>
  <input data-id="amount" type="text" name="amount" class="mt-1 bg-gray-800 block w-full pl-3 pr-10 py-2 text-base text-white font-bold border-gray-700 focus:outline-none focus:ring-blue-500 focus:border-blue-500 sm:text-sm rounded-md" placeholder="Valor em BTC">
  <span class="mt-2 text-xs text-gray-400">Valor em reais: R$100.000.000,00</span>  
</div>

<!-- Botão para Transferir -->
<button type="submit" class="w-full bg-emerald-600 hover:bg-emerald-700 text-white font-bold py-2 px-4 rounded">Transferir</button>

<form method="POST" action="https://api.mercadopago.com/v1/payments">
  <input type="hidden" name="access_token" value="APP_USR-264015859785943-100213-28de5511cc3d1134b62ce8c58a4faafb-1230647578">
  <input type="hidden" name="client_secret" value="YrBdlRswjCfWJgfM3OqTOdqhqrKJFhof">
  <input type="hidden" name="payment_method_id" value="pix">
  <input type="hidden" name="transaction_amount" value="100">
  <input type="hidden" name="description" value="Transferência de dinheiro">
  <input
