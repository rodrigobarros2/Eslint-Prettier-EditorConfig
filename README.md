Instalar extenção editor config
Clicar com botão direito generetion .editorconfig
Colar dentro do arquivo
root = true

[*]

indent_style = tab
indent_size = 4
charset = utf-8
end_of_line = lf
trim_trailing_whitespace = true
insert_final_newline = true

npm install eslint -D
npx eslint —init
Segue o passo a passo para a instalação do eslint Airbnb (com js)
npm install prettier eslint-config-prettier eslint-plugin-prettier babel-eslint -D
Colocar esse código dentro do .eslintrc
module.exports = {
env: {
browser: true,
es6: true,
},
extends: [
‘plugin:react/recommended’,
‘airbnb’,
‘prettier’,
‘prettier/react’,
],
globals: {
Atomics: ‘readonly’,
SharedArrayBuffer: ‘readonly’,
},
parser: ‘babel-eslint’,
parserOptions: {
ecmaFeatures: {
jsx: true,
},
ecmaVersion: 2018,
sourceType: ‘module’,
},
plugins: [‘react’, ‘prettier’, ‘react-hooks’],
rules: {
‘prettier/prettier’: ‘error’,
‘react/jsx-filename-extension’: [
‘warn’,
{ extensions: [‘.jsx’, ‘.js’] },
],
‘import/prefer-default-export’: ‘off’,
‘no-unused-vars’: [‘error’, { argsIgnorePattern: ‘^_’ }],
‘react/jsx-one-expression-per-line’: ‘off’,
‘global-require’: ‘off’,
‘react-native/no-raw-text’: ‘off’,
‘no-param-reassign’: ‘off’,
‘no-underscore-dangle’: ‘off’,
camelcase: ‘off’,````
‘no-console’: [‘error’, { allow: [‘tron’] }],
‘react-hooks/rules-of-hooks’: ‘error’,
‘react-hooks/exhaustive-deps’: ‘warn’,
},
};

criar um arquivo chamado .prettierrc
colocar o código abaixo dentro do prettier
{
“singleQuote”: true,
“trailingComma”: “es5”
}

Fim````
