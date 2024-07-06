
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Учет расходов и доходов</title>
    <link rel="stylesheet" href="my.css" />
  </head>
  <body>
    <div class="container">
      <h1>Учет расходов и доходов</h1>

      <div class="flex-container">
        <div class="transactions">
          <h2>Транзакции</h2>
          <div id="transactionsList"></div>
          <form id="transactionForm">
            <h3>Добавить транзакцию</h3>
            <label for="transactionType">Тип транзакции:</label>
            <select id="transactionType">
              <option value="income">Доход</option>
              <option value="expense">Расход</option></select
            ><br />
            <label for="transactionAmount">Сумма:</label>
            <input
              type="number"
              id="transactionAmount"
              step="0.01"
              required
            /><br />
            <label for="transactionCategory">Категория:</label>
            <select id="transactionCategory"></select
            ><br />
            <label for="transactionAccount">Счет:</label>
            <select id="transactionAccount"></select
            ><br />
            <label for="transactionComment">Комментарий:</label>
            <input type="text" id="transactionComment" /><br />
            <label for="transactionDate">Дата:</label>
            <input type="date" id="transactionDate" /><br />
            <button type="submit">Добавить транзакцию</button>
          </form>
        </div>

        <div class="accounts">
          <h2>Счета и балансы</h2>
          <ul id="accountsList"></ul>

          <div id="balanceChange">
            <h3>Изменение баланса</h3>
            <form id="balanceForm">
              <label for="accountSelect">Выберите счет:</label>
              <select id="accountSelect"></select
              ><br />
              <label for="changeAmount"
                >Введите сумму для изменения баланса:</label
              >
              <input
                type="number"
                id="changeAmount"
                step="0.01"
                required
              /><br />
              <button type="submit">Изменить баланс</button>
            </form>
          </div>

          <div id="addAccount">
            <h3>Добавить новый счет</h3>
            <form id="accountForm">
              <label for="newAccountName">Название нового счета:</label>
              <input type="text" id="newAccountName" required />
              <button type="submit">Добавить счет</button>
            </form>
          </div>
        </div>
      </div>
    </div>

    <script src="my.js"></script>
  </body>
</html>
