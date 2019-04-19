// merge 2 objects

function merge2Object(src, des) {
  const keys = Object.keys(des);
  for (const key of keys) {
    if (src[key] === undefined || typeof src[key] !== 'object' || typeof des[key] !== 'object') {
      src[key] = des[key];
    } else if (typeof src[key] === 'object' && typeof des[key] === 'object') {
      merge2Object(src[key], des[key]);
    } else if (typeof src[key] !== 'object') {
      src[key] = des[key];
    }
  }
}
