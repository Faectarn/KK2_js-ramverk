<style>
@import url("https://fonts.googleapis.com/css2?family=Combo&display=swap");

body {
  margin: 0;
  color: rgb(229, 229, 233);
  background: #14181c;
}

main {
  margin: 0 auto;
  width: 25rem;
  padding: 2rem 3rem;
  background: rgba(255, 255, 255, 0.1);
  backdrop-filter: blur(10px);
  box-shadow: rgba(0, 0, 0, 0.15) 2px 2px 2.5px;
  border-radius: 10px;
}

h1 {
  margin: 3rem 0 2rem 0;
}

.top {
  display: flex;
  margin-bottom: 1rem;
}

.inputField {
  font-family: "Combo", cursive;
  font-size: 20px;
  width: 100%;
  padding: 0.8rem;
  border: 1px solid rgb(146, 146, 146);
  border-radius: 5px;
  box-shadow: rgb(0 0 0 / 15%) 2px 2px 2.5px;
}

button {
  cursor: pointer;
  border: none;
}

.add {
  padding: 5px 18px;
  margin-left: 10px;
  font-size: 36px;
  background: linear-gradient(45deg, rgb(38, 97, 24), rgb(12, 163, 32));
  border-radius: 5px;
  box-shadow: rgb(0 0 0 / 15%) 2px 2px 2.5px;
}

span {
  margin-left: 10px;
}

.listItem {
  display: flex;
  align-items: center;
  margin: 2rem 0;
  font-size: 20px;
  font-weight: bold;
}

.done {
  transform: scale(1.5);
}

.completed {
  text-decoration: line-through;
  opacity: 0.7;
}

.delete {
  margin-left: auto;
  background: transparent;
  font-size: 15px;
}
</style>