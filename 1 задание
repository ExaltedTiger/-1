// Класс схемы для проверки email
class EmailSchema {
  isValid(value) {
    // 1. Проверяем, что значение является строкой
    if (typeof value !== 'string') {
      return false;
    }
    // 2. Проверяем наличие символа '@' (согласно условию задачи)
    return value.includes('@');
  }
}

// Основной класс валидатора
class Validator {
  email() {
    // Возвращаем новый экземпляр схемы для email
    return new EmailSchema();
  }
}

// --- Тестирование (как в примере) ---
const v = new Validator();
const emailSchema = v.email();

console.log(emailSchema.isValid('invalid-email'));          // false
console.log(emailSchema.isValid('valid.email@e  xmaple.com')); // true
console.log(emailSchema.isValid('valid.email@vovovo.ru'));  // true
console.log(emailSchema.isValid('valid.email@pepepe.eu'));  // true
console.log(emailSchema.isValid('another.valid@123.45'));   // true
console.log(emailSchema.isValid(15613854));                 // false
console.log(emailSchema.isValid(''));                       // false
