# CRUD---Parte-4

Atualização das políticas se necessário:

<code>-- Ativa o RLS na tabela
ALTER TABLE public.produtos ENABLE ROW LEVEL SECURITY;

-- Cria a política permitindo que qualquer um (anon) faça SELECT
CREATE POLICY "Permitir leitura publica" 
ON public.produtos FOR SELECT 
TO public
USING (true);</code>
