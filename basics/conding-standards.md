### Java Coding Standards

Whenever we are writing any component. Its name should reflect the purpose of that component (functionality), this helps in readability and maintability of the code. 

**Class Coding Standards**
- Usually a Noun. Ex Account, String.
- Should start with uppercase characters and in case of multiple words. Every inner word should start with upper case character i.e PascalCase. Example: StringBuffer, AccountDetails.

**Interface Coding Standards**
- Usually an adjective. Example: Runnable, Serializable.
- Should start with uppercase characters and in case of multiple words. Every inner word should start with upper case character i.e PascalCase.

**Method Coding Standards**
- Usually a verb or a verb noun combination. Example sleep(), run(), getAccountId(), setSalary()
- Starts with lower case but every inner word starts with upper case i.e camelCase convention. Example getAccountId()

**Variable Coding Standards**
- Usually a Noun. Example accountId, mobileNumber.
- Follows camelCase convention. Example accountId, accountHolderName.

**Constants Coding Standards**
- Usually a Noun.
- Should contain only upper case characters and in case of multiple words than the words are separated with underscore symbol. Example MAX_VALUE, MIN_PRIORITY
- Usually we can declare constants with `public static final` modifiers
