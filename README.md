import {
  Project,
  Sprite,
} from "https://unpkg.com/leopard@^1/dist/index.esm.js";

import Stage from "./Stage/Stage.js";
import Appel from "./Appel/Appel.js";
import Level from "./Level/Level.js";
import LevelCompleted from "./LevelCompleted/LevelCompleted.js";
import Hint from "./Hint/Hint.js";
import Sprite1 from "./Sprite1/Sprite1.js";
import Blustryx8ExplosionEffect from "./Blustryx8ExplosionEffect/Blustryx8ExplosionEffect.js";
import Sprite2 from "./Sprite2/Sprite2.js";
import Sprite3 from "./Sprite3/Sprite3.js";

const stage = new Stage({ costumeNumber: 1 });

const sprites = {
  Appel: new Appel({
    x: -190,
    y: -50,
    direction: 90,
    rotationStyle: Sprite.RotationStyle.LEFT_RIGHT,
    costumeNumber: 2,
    size: 100,
    visible: true,
    layerOrder: 2,
  }),
  Level: new Level({
    x: 0,
    y: 0,
    direction: 90,
    rotationStyle: Sprite.RotationStyle.ALL_AROUND,
    costumeNumber: 1,
    size: 100,
    visible: true,
    layerOrder: 1,
  }),
  LevelCompleted: new LevelCompleted({
    x: 0,
    y: 0,
    direction: 90,
    rotationStyle: Sprite.RotationStyle.ALL_AROUND,
    costumeNumber: 5,
    size: 100,
    visible: false,
    layerOrder: 3,
  }),
  Hint: new Hint({
    x: 0,
    y: 0,
    direction: 90,
    rotationStyle: Sprite.RotationStyle.ALL_AROUND,
    costumeNumber: 1,
    size: 100,
    visible: false,
    layerOrder: 5,
  }),
  Sprite1: new Sprite1({
    x: 0,
    y: 0,
    direction: 90,
    rotationStyle: Sprite.RotationStyle.ALL_AROUND,
    costumeNumber: 11,
    size: 100,
    visible: false,
    layerOrder: 4,
  }),
  Blustryx8ExplosionEffect: new Blustryx8ExplosionEffect({
    x: -106.13864452806448,
    y: -70.45125740286477,
    direction: 90,
    rotationStyle: Sprite.RotationStyle.ALL_AROUND,
    costumeNumber: 1,
    size: 100,
    visible: true,
    layerOrder: 6,
  }),
  Sprite2: new Sprite2({
    x: 0,
    y: 60,
    direction: 90,
    rotationStyle: Sprite.RotationStyle.ALL_AROUND,
    costumeNumber: 1,
    size: 100,
    visible: true,
    layerOrder: 7,
  }),
  Sprite3: new Sprite3({
    x: -60,
    y: -40,
    direction: 90,
    rotationStyle: Sprite.RotationStyle.ALL_AROUND,
    costumeNumber: 1,
    size: 100,
    visible: true,
    layerOrder: 8,
  }),
};

const project = new Project(stage, sprites, {
  frameRate: 30, // Set to 60 to make your project run faster
});
export default project;
