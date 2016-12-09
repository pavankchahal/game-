<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Snake | Rembound</title>
<script type="text/javascript">
document.onkeydown = function(evt) {
    evt = evt || window.event;
    var keyCode = evt.keyCode;
    if (keyCode >= 37 && keyCode <= 40 || keyCode == 32) {
        return false;
    }
};
</script>
<script>
 
window.onload = function() {
  var m = document.getElementById("viewport");
  var K = m.getContext("2d");
  var F = 0;
  var v = 0;
  var A = 0;
  var x = 0;
  var o = false;
  var c = [];
  var h;
  var t = 0;
  var i = 0;
  var z = false;

  function g(O) {
    t = 0;
    i = O.length;
    z = false;
    var L = [];
    for (var M = 0; M < O.length; M++) {
      var N = new Image();
      N.onload = function() {
        t++;
        if (t == i) {
          z = true
        }
      };
      N.src = O[M];
      L[M] = N
    }
    return L
  }
  var J = function(P, Q, O, M) {
    this.columns = P;
    this.rows = Q;
    this.tilewidth = O;
    this.tileheight = M;
    this.tiles = [];
    for (var N = 0; N < this.columns; N++) {
      this.tiles[N] = [];
      for (var L = 0; L < this.rows; L++) {
        this.tiles[N][L] = 0
      }
    }
  };
  J.prototype.generate = function() {
    for (var M = 0; M < this.columns; M++) {
      for (var L = 0; L < this.rows; L++) {
        if (M == 0 || M == this.columns - 1 || L == 0 || L == this.rows - 1) {
          this.tiles[M][L] = 1
        } else {
          this.tiles[M][L] = 0
        }
      }
    }
  };
  var n = function() {
    this.init(0, 0, 1, 10, 1)
  };
  n.prototype.directions = [
    [0, -1],
    [1, 0],
    [0, 1],
    [-1, 0]
  ];
  n.prototype.init = function(L, Q, P, O, N) {
    this.x = L;
    this.y = Q;
    this.direction = P;
    this.speed = O;
    this.movedelay = 0;
    this.segments = [];
    this.growsegments = 0;
    for (var M = 0; M < N; M++) {
      this.segments.push({
        x: this.x - M * this.directions[P][0],
        y: this.y - M * this.directions[P][1]
      })
    }
  };
  n.prototype.grow = function() {
    this.growsegments++
  };
  n.prototype.tryMove = function(M) {
    this.movedelay += M;
    var L = 1 / this.speed;
    if (this.movedelay > L) {
      return true
    }
    return false
  };
  n.prototype.nextMove = function() {
    var M = this.x + this.directions[this.direction][0];
    var L = this.y + this.directions[this.direction][1];
    return {
      x: M,
      y: L
    }
  };
  n.prototype.move = function() {
    var P = this.nextMove();
    this.x = P.x;
    this.y = P.y;
    var L = this.segments[this.segments.length - 1];
    var O = L.x;
    var M = L.y;
    for (var N = this.segments.length - 1; N >= 1; N--) {
      this.segments[N].x = this.segments[N - 1].x;
      this.segments[N].y = this.segments[N - 1].y
    }
    if (this.growsegments > 0) {
      this.segments.push({
        x: O,
        y: M
      });
      this.growsegments--
    }
    this.segments[0].x = this.x;
    this.segments[0].y = this.y;
    this.movedelay = 0
  };
  var y = new n();
  var j = new J(20, 15, 32, 32);
  var b = 0;
  var E = true;
  var q = 1;
  var r = 0.5;

  function H() {
    c = g(["snake-graphics.png"]);
    h = c[0];
    m.addEventListener("mousedown", I);
    document.addEventListener("keydown", l);
    e();
    E = true;
    d(0)
  }

  function k() {
    if (q > r) {
      e();
      E = false
    }
  }

  function e() {
    y.init(10, 10, 1, 10, 4);
    j.generate();
    u();
    b = 0;
    E = false
  }

  function u() {
    var O = false;
    while (!O) {
      var P = a(0, j.columns - 1);
      var N = a(0, j.rows - 1);
      var L = false;
      for (var M = 0; M < y.segments.length; M++) {
        var R = y.segments[M].x;
        var Q = y.segments[M].y;
        if (P == R && N == Q) {
          L = true;
          break
        }
      }
      if (!L && j.tiles[P][N] == 0) {
        j.tiles[P][N] = 2;
        O = true
      }
    }
  }

  function d(N) {
    window.requestAnimationFrame(d);
    if (!o) {
      K.clearRect(0, 0, m.width, m.height);
      var L = t / i;
      K.strokeStyle = "#ff8080";
      K.lineWidth = 3;
      K.strokeRect(18.5, 0.5 + m.height - 51, m.width - 37, 32);
      K.fillStyle = "#ff8080";
      K.fillRect(18.5, 0.5 + m.height - 51, L * (m.width - 37), 32);
      var M = "Loaded " + t + "/" + i + " images";
      K.fillStyle = "#000000";
      K.font = "16px Verdana";
      K.fillText(M, 18, 0.5 + m.height - 63);
      if (z) {
        o = true
      }
    } else {
      D(N);
      C()
    }
  }

  function D(L) {
    var M = (L - F) / 1000;
    F = L;
    G(M);
    if (!E) {
      B(M)
    } else {
      q += M
    }
  }

  function B(N) {
    if (y.tryMove(N)) {
      var P = y.nextMove();
      var L = P.x;
      var R = P.y;
      if (L >= 0 && L < j.columns && R >= 0 && R < j.rows) {
        if (j.tiles[L][R] == 1) {
          E = true
        }
        for (var M = 0; M < y.segments.length; M++) {
          var Q = y.segments[M].x;
          var O = y.segments[M].y;
          if (L == Q && R == O) {
            E = true;
            break
          }
        }
        if (!E) {
          y.move();
          if (j.tiles[L][R] == 2) {
            j.tiles[L][R] = 0;
            u();
            y.grow();
            b++
          }
        }
      } else {
        E = true
      }
      if (E) {
        q = 0
      }
    }
  }

  function G(L) {
    if (v > 0.25) {
      x = Math.round(A / v);
      v = 0;
      A = 0
    }
    v += L;
    A++
  }

  function C() {
    K.fillStyle = "#577ddb";
    K.fillRect(0, 0, m.width, m.height);
    f();
    w();
    if (E) {
      K.fillStyle = "rgba(0, 0, 0, 0.5)";
      K.fillRect(0, 0, m.width, m.height);
      K.fillStyle = "#ffffff";
      K.font = "24px Verdana";
      p("Press any key to start!", 0, m.height / 2, m.width)
    }
  }

  function f() {
    for (var O = 0; O < j.columns; O++) {
      for (var M = 0; M < j.rows; M++) {
        var R = j.tiles[O][M];
        var S = O * j.tilewidth;
        var Q = M * j.tileheight;
        if (R == 0) {
          K.fillStyle = "#f7e697";
          K.fillRect(S, Q, j.tilewidth, j.tileheight)
        } else {
          if (R == 1) {
            K.fillStyle = "#bcae76";
            K.fillRect(S, Q, j.tilewidth, j.tileheight)
          } else {
            if (R == 2) {
              K.fillStyle = "#f7e697";
              K.fillRect(S, Q, j.tilewidth, j.tileheight);
              var P = 0;
              var N = 3;
              var T = 64;
              var L = 64;
              K.drawImage(h, P * T, N * L, T, L, S, Q, j.tilewidth, j.tileheight)
            }
          }
        }
      }
    }
  }

  function w() {
    for (var N = 0; N < y.segments.length; N++) {
      var P = y.segments[N];
      var U = P.x;
      var T = P.y;
      var R = U * j.tilewidth;
      var Q = T * j.tileheight;
      var O = 0;
      var M = 0;
      if (N == 0) {
        var S = y.segments[N + 1];
        if (T < S.y) {
          O = 3;
          M = 0
        } else {
          if (U > S.x) {
            O = 4;
            M = 0
          } else {
            if (T > S.y) {
              O = 4;
              M = 1
            } else {
              if (U < S.x) {
                O = 3;
                M = 1
              }
            }
          }
        }
      } else {
        if (N == y.segments.length - 1) {
          var L = y.segments[N - 1];
          if (L.y < T) {
            O = 3;
            M = 2
          } else {
            if (L.x > U) {
              O = 4;
              M = 2
            } else {
              if (L.y > T) {
                O = 4;
                M = 3
              } else {
                if (L.x < U) {
                  O = 3;
                  M = 3
                }
              }
            }
          }
        } else {
          var L = y.segments[N - 1];
          var S = y.segments[N + 1];
          if (L.x < U && S.x > U || S.x < U && L.x > U) {
            O = 1;
            M = 0
          } else {
            if (L.x < U && S.y > T || S.x < U && L.y > T) {
              O = 2;
              M = 0
            } else {
              if (L.y < T && S.y > T || S.y < T && L.y > T) {
                O = 2;
                M = 1
              } else {
                if (L.y < T && S.x < U || S.y < T && L.x < U) {
                  O = 2;
                  M = 2
                } else {
                  if (L.x > U && S.y < T || S.x > U && L.y < T) {
                    O = 0;
                    M = 1
                  } else {
                    if (L.y > T && S.x > U || S.y > T && L.x > U) {
                      O = 0;
                      M = 0
                    }
                  }
                }
              }
            }
          }
        }
      }
      K.drawImage(h, O * 64, M * 64, 64, 64, R, Q, j.tilewidth, j.tileheight)
    }
  }

  function p(O, L, P, N) {
    var M = K.measureText(O);
    K.fillText(O, L + (N - M.width) / 2, P)
  }

  function a(L, M) {
    return Math.floor(L + Math.random() * (M - L + 1))
  }

  function I(L) {
    var M = s(m, L);
    if (E) {
      k()
    } else {
      y.direction = (y.direction + 1) % y.directions.length
    }
  }

  function l(L) {
    if (E) {
      k()
    } else {
      if (L.keyCode == 37 || L.keyCode == 65) {
        if (y.direction != 1) {
          y.direction = 3
        }
      } else {
        if (L.keyCode == 38 || L.keyCode == 87) {
          if (y.direction != 2) {
            y.direction = 0
          }
        } else {
          if (L.keyCode == 39 || L.keyCode == 68) {
            if (y.direction != 3) {
              y.direction = 1
            }
          } else {
            if (L.keyCode == 40 || L.keyCode == 83) {
              if (y.direction != 0) {
                y.direction = 2
              }
            }
          }
        }
      }
      if (L.keyCode == 32) {
        y.grow()
      }
    }
  }

  function s(L, N) {
    var M = L.getBoundingClientRect();
    return {
      x: Math.round((N.clientX - M.left) / (M.right - M.left) * L.width),
      y: Math.round((N.clientY - M.top) / (M.bottom - M.top) * L.height)
    }
  }
  H()
};
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Snake | Rembound</title>
<script type="text/javascript">
document.onkeydown = function(evt) {
    evt = evt || window.event;
    var keyCode = evt.keyCode;
    if (keyCode >= 37 && keyCode <= 40 || keyCode == 32) {
        return false;
    }
};
</script>
</body>
</html> 
