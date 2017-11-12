namespace NuevoPolito.Migrations
{
    using NuevoPolito.Models;
    using System;
    using System.Data.Entity;
    using System.Data.Entity.Migrations;
    using System.Linq;

    internal sealed class Configuration : DbMigrationsConfiguration<NuevoPolito.Models.ApplicationDbContext>
    {
        public Configuration()
        {
            AutomaticMigrationsEnabled = false;
            ContextKey = "NuevoPolito.Models.ApplicationDbContext";
        }

        protected override void Seed(NuevoPolito.Models.ApplicationDbContext context)
        {
            //  This method will be called after migrating to the latest version.

            //  You can use the DbSet<T>.AddOrUpdate() helper extension method 
            //  to avoid creating duplicate seed data. E.g.
            //
            //    context.People.AddOrUpdate(
            //      p => p.FullName,
            //      new Person { FullName = "Andrew Peters" },
            //      new Person { FullName = "Brice Lambson" },
            //      new Person { FullName = "Rowan Miller" }
            //    );
            //
            context.Departamentos.AddOrUpdate(
            a => a.Id,
                new Departamento { Id = 1, Codigo = "91", Nombre = "Antioquia" }
               
            );
            context.Ciudades.AddOrUpdate(
            a => a.Id,
                new Ciudad { Id = 10, Codigo = "05120", Nombre = "CÁCERES", DepartamentoId = 1 },
                new Ciudad { Id = 11, Codigo = "05154", Nombre = "CAUCASIA", DepartamentoId = 1 },
                new Ciudad { Id = 12, Codigo = "05250", Nombre = "EL BAGRE", DepartamentoId = 1 },
                new Ciudad { Id = 13, Codigo = "05495", Nombre = "NECHÍ", DepartamentoId = 1 },
                new Ciudad { Id = 14, Codigo = "05790", Nombre = "TARAZÁ", DepartamentoId = 1 },
                new Ciudad { Id = 15, Codigo = "05895", Nombre = "ZARAGOZA", DepartamentoId = 1 },
                new Ciudad { Id = 16, Codigo = "05142", Nombre = "CARACOLÍ", DepartamentoId = 1 },
                new Ciudad { Id = 17, Codigo = "05425", Nombre = "MACEO", DepartamentoId = 1 },
                new Ciudad { Id = 18, Codigo = "05579", Nombre = "PUERTO BERRiO", DepartamentoId = 1 },
                new Ciudad { Id = 19, Codigo = "05585", Nombre = "PUERTO NARE", DepartamentoId = 1 },
                new Ciudad { Id = 20, Codigo = "05591", Nombre = "PUERTO TRIUNFO", DepartamentoId = 1 },
                new Ciudad { Id = 21, Codigo = "05893", Nombre = "YONDÓ", DepartamentoId = 1 },
                new Ciudad { Id = 22, Codigo = "05031", Nombre = "AMALFI", DepartamentoId = 1 },
                new Ciudad { Id = 23, Codigo = "05040", Nombre = "ANORÍ", DepartamentoId = 1 },
                new Ciudad { Id = 24, Codigo = "05190", Nombre = "CISNEROS", DepartamentoId = 1 },
                new Ciudad { Id = 25, Codigo = "05604", Nombre = "REMEDIOS", DepartamentoId = 1 },
                new Ciudad { Id = 26, Codigo = "05670", Nombre = "SAN ROQUE", DepartamentoId = 1 },
                new Ciudad { Id = 27, Codigo = "05690", Nombre = "SANTO DOMINGO", DepartamentoId = 1 },
                new Ciudad { Id = 28, Codigo = "05736", Nombre = "SEGOVIA", DepartamentoId = 1 },
                new Ciudad { Id = 29, Codigo = "05858", Nombre = "VEGACHÍ", DepartamentoId = 1 },
                new Ciudad { Id = 30, Codigo = "05885", Nombre = "YALÍ", DepartamentoId = 1 },
                new Ciudad { Id = 31, Codigo = "05890", Nombre = "YOLOMBÓ", DepartamentoId = 1 },
                new Ciudad { Id = 32, Codigo = "05038", Nombre = "ANGOSTURA", DepartamentoId = 1 },
                new Ciudad { Id = 33, Codigo = "05086", Nombre = "BELMIRA", DepartamentoId = 1 },
                new Ciudad { Id = 34, Codigo = "05107", Nombre = "BRICEÑO", DepartamentoId = 1 },
                new Ciudad { Id = 35, Codigo = "05134", Nombre = "CAMPAMENTO", DepartamentoId = 1 },
                new Ciudad { Id = 36, Codigo = "05150", Nombre = "CAROLINA", DepartamentoId = 1 },
                new Ciudad { Id = 37, Codigo = "05237", Nombre = "DON MATiAS", DepartamentoId = 1 },
                new Ciudad { Id = 38, Codigo = "05264", Nombre = "ENTRERRIOS", DepartamentoId = 1 },
                new Ciudad { Id = 39, Codigo = "05310", Nombre = "GÓMEZ PLATA", DepartamentoId = 1 },
                new Ciudad { Id = 40, Codigo = "05315", Nombre = "GUADALUPE", DepartamentoId = 1 },
                new Ciudad { Id = 41, Codigo = "05361", Nombre = "ITUANGO", DepartamentoId = 1 },
                new Ciudad { Id = 42, Codigo = "05647", Nombre = "SAN ANDRÉS", DepartamentoId = 1 },
                new Ciudad { Id = 43, Codigo = "05658", Nombre = "SAN JOSÉ DE LA MONTA", DepartamentoId = 1 },
                new Ciudad { Id = 44, Codigo = "05664", Nombre = "SAN PEDRO", DepartamentoId = 1 },
                new Ciudad { Id = 45, Codigo = "05686", Nombre = "SANTA ROSA de osos", DepartamentoId = 1 },
                new Ciudad { Id = 46, Codigo = "05819", Nombre = "TOLEDO", DepartamentoId = 1 },
                new Ciudad { Id = 47, Codigo = "05854", Nombre = "VALDIVIA", DepartamentoId = 1 },
                new Ciudad { Id = 48, Codigo = "05887", Nombre = "YARUMAL", DepartamentoId = 1 },
                new Ciudad { Id = 49, Codigo = "05004", Nombre = "ABRIAQUÍ", DepartamentoId = 1 },
                new Ciudad { Id = 50, Codigo = "05044", Nombre = "ANZA", DepartamentoId = 1 },
                new Ciudad { Id = 51, Codigo = "05059", Nombre = "ARMENIA", DepartamentoId = 1 },
                new Ciudad { Id = 52, Codigo = "05113", Nombre = "BURITICÁ", DepartamentoId = 1 },
                new Ciudad { Id = 53, Codigo = "05138", Nombre = "CAÑASGORDAS", DepartamentoId = 1 },
                new Ciudad { Id = 54, Codigo = "05234", Nombre = "DABEIBA", DepartamentoId = 1 },
                new Ciudad { Id = 55, Codigo = "05240", Nombre = "EBÉJICO", DepartamentoId = 1 },
                new Ciudad { Id = 56, Codigo = "05284", Nombre = "FRONTINO", DepartamentoId = 1 },
                new Ciudad { Id = 57, Codigo = "05306", Nombre = "GIRALDO", DepartamentoId = 1 },
                new Ciudad { Id = 58, Codigo = "05347", Nombre = "HELICONIA", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05411", Nombre = "LIBORINA", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05501", Nombre = "OLAYA", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05543", Nombre = "PEQUE", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05628", Nombre = "SABANALARGA", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05656", Nombre = "SAN JERÓNIMO", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05042", Nombre = "SANTAFÉ DE ANTIOQUIAS", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05761", Nombre = "SOPETRaN", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05842", Nombre = "URAMITA", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05002", Nombre = "ABEJORRAL", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05021", Nombre = "ALEJANDRÍA", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05055", Nombre = "ARGELIA", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05148", Nombre = "CARMEN DE VIBORAL", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05197", Nombre = "COCORNÁ", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05206", Nombre = "CONCEPCIÓN", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05313", Nombre = "GRANADA", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05318", Nombre = "GUARNE", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05321", Nombre = "GUATAPE", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05376", Nombre = "LA CEJA", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05400", Nombre = "LA UNIÓN", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05440", Nombre = "MARINILLA", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05483", Nombre = "NARIÑO", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05541", Nombre = "PEÑOL", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05607", Nombre = "RETIRO", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05615", Nombre = "RIONEGRO", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05649", Nombre = "SAN CARLOS", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05652", Nombre = "SAN FRANCISCO", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05660", Nombre = "SAN LUIS", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05667", Nombre = "SAN RAFAEL", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05674", Nombre = "SAN VICENTE", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05697", Nombre = "SANTUARIO", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05756", Nombre = "SONSON", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05030", Nombre = "AMAGa", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05034", Nombre = "ANDES", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05036", Nombre = "ANGELOPOLIS", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05091", Nombre = "BETANIA", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05093", Nombre = "BETULIA", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05125", Nombre = "CAICEDO", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05145", Nombre = "CARAMANTA", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05101", Nombre = "CIUDAD BOLÍVAR", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05209", Nombre = "CONCORDIA", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05282", Nombre = "FREDONIA", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05353", Nombre = "HISPANIA", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05364", Nombre = "JARDÍN", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05368", Nombre = "JERICÓ", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05390", Nombre = "LA PINTADA", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05467", Nombre = "MONTEBELLO", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05576", Nombre = "PUEBLORRICO", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05642", Nombre = "SALGAR", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05679", Nombre = "SANTA BaRBARA", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05789", Nombre = "TÁMESIS", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05792", Nombre = "TARSO", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05809", Nombre = "TITIRIBÍ", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05847", Nombre = "URRAO", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05856", Nombre = "VALPARAISO", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05861", Nombre = "VENECIA", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05045", Nombre = "APARTADÓ", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05051", Nombre = "ARBOLETES", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05147", Nombre = "CAREPA", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05172", Nombre = "CHIGORODÓ", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05475", Nombre = "MURINDÓ", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05480", Nombre = "MUTATA", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05490", Nombre = "NECOCLÍ", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05659", Nombre = "SAN JUAN DE URABA", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05665", Nombre = "SAN PEDRO DE URABA", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05837", Nombre = "TURBO", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05873", Nombre = "VIGÍA DEL FUERTE", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05079", Nombre = "BARBOSA", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05088", Nombre = "BELLO", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05129", Nombre = "CALDAS", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05212", Nombre = "COPACABANA", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05266", Nombre = "ENVIGADO", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05308", Nombre = "GIRARDOTA", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05360", Nombre = "ITAGUI", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05380", Nombre = "LA ESTRELLA", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05001", Nombre = "MEDELLÍN", DepartamentoId = 1 },
                new Ciudad { Id = 59, Codigo = "05631", Nombre = "SABANETA", DepartamentoId = 1 }
            );
        }
    }
}
