<template>
    <h3>Edit your character</h3>
    <form>
      <section>
        <label for="name">Name</label>
        <input type="text" placeholder="Name" id="name" />
      </section>
      <section>
        <label for="level">Level</label>
        <input type="number" min="0" placeholder="Level" id="level" />
      </section>
      <section>
        <label>Job:</label>
        <select>
          <option value="fighter">Fighter</option>
          <option value="ranger">Ranger</option>
          <option value="sorcerer">Sorcerer</option>
        </select>
      </section>
      <section>
        <label>Race:</label>
        <input type="radio" name="race" id="human" value="human" />
        <label for="human">Human</label>
        <input type="radio" name="race" id="elf" value="elf" />
        <label for="elf">Elf</label>
        <input type="radio" name="race" id="orc" value="orc" />
        <label for="orc">Orc</label>
      </section>
      <section>
        <label for="bio">Bio</label>
        <textarea id="bio" rows="3"></textarea>
      </section>
    </form>
  </template>
  
  <style scoped>
  form {
    background: #ffffffaa;
    padding: 25px;
  }
  
  form section + section {
    margin: 10px 0;
  }
  
  form section label {
    color: black;
  }
  
  form section label:first-child {
    display: inline-block;
    width: 15%;
  }
  
  form section label:not(first-child) {
    margin-right: 10px;
  }
  
  form section input[type='text'],
  form section input[type='number'],
  form section select,
  form section textarea {
    padding: 5px;
    width: 70%;
  }
  </style>
  